# cinescore - 🎬 IMDb Movie Rating Predictor (Indian Movies)

**Cinescore - IMDb Movie Rating Predictor** is a **machine learning web application** project designed to predict the IMDb rating of Indian movies based on various attributes like year, duration, genre, director, and actors.
The project uses Random Forest Regression and provides an interactive **Streamlit interface** for real-time predictions.

## 🚀 Features

- Data Preprocessing – Cleans and formats IMDb dataset (handles missing values, standardizes text, extracts year/duration)
- Categorical Encoding – Encodes directors and actors using Label Encoding
- Genre Feature Engineering – Creates binary columns for each genre from multi-genre entries
- Model Training – Trains a Random Forest Regressor on cleaned data
- Model Saving – Stores trained model, encoders, and feature columns in a pickle file
- Interactive Web App – Built with Streamlit for easy predictions
- Real-time Rating Prediction – Predicts IMDb rating based on user inputs
- User Feedback & Visuals – Displays prediction result, progress bar, and feedback messages (blockbuster, promising, needs improvement)

## 📂 Project Structure

- ├── movie_preprocess.py     # Script for cleaning and preprocessing raw IMDb dataset
- ├── movie_train.py          # Script for training Random Forest model
- ├── movie_test.py           # Streamlit app for testing/predicting ratings
- ├── Cleaned_IMDb_Movies_India.csv  # Cleaned dataset
- ├── movie_model.pkl         # Saved trained model and encoders
- ├── README.md               # Project documentation

## 🛠 Tech Stack

- Python
- Pandas – Data cleaning and preprocessing
- Scikit-learn – Model training and encoding
- Random Forest Regressor – Rating prediction model
- Streamlit – Web application interface
- Pickle – Model and encoder serialization

## 🔍 How It Works

1. Data Preprocessing (movie_preprocess.py)
Cleans column names and missing values
Extracts Year and Duration from strings
Fills missing categorical fields with "Unknown"
Converts votes and ratings to numeric values
Saves cleaned dataset as Cleaned_IMDb_Movies_India.csv

2. Model Training (movie_train.py)
Encodes categorical features (Director, Actor 1–3)
One-hot encodes genres into binary columns
Selects relevant features and trains Random Forest
Saves model, encoders, genres, and feature list to movie_model.pkl

3. Prediction Web App (movie_test.py)
Loads saved model and encoders
Takes user inputs for year, duration, genre, director, and actors
Encodes features and predicts rating in real-time
Displays result with rating scale and feedback

## 🖥 How to Run

### 1️⃣ Clone the Repo
git clone https://github.com/yourusername/imdb-movie-rating-predictor.git
cd imdb-movie-rating-predictor
### 2️⃣ Install Requirements
pip install pandas scikit-learn streamlit numpy
### 3️⃣ Run Preprocessing
python movie_preprocess.py
### 4️⃣ Train Model
python movie_train.py
### 5️⃣ Run Web App
streamlit run movie_test.py

## 💡 Use Cases

- Pre-release Rating Forecast – Predict a movie’s potential IMDb rating before release based on cast, crew, and genre.
- Script & Casting Decisions – Help producers decide on directors and actors likely to improve audience ratings.
- Market Research for Distributors – Identify movies with higher predicted ratings for better marketing investment.
- Festival & Award Strategy – Gauge potential critical reception for award submissions.
- Audience Engagement Tools – Build interactive apps where fans guess or compare ratings with model predictions.
- Trend Analysis – Track changes in predicted ratings based on cast/crew combinations over time.
- Content Recommendation – Suggest similar high-rated movies for streaming platforms.

## 👩‍💻 Author
**Devadarshini P**  
[🔗 LinkedIn](https://www.linkedin.com/in/devadarshini-p-707b15202/)  
[💻 GitHub](https://github.com/Devadarshini9000)

"Predict the stars before they shine – let data decide the box office." 🎬⭐

<img width="800" height="787" alt="image" src="https://github.com/user-attachments/assets/021a74b4-b7e9-4200-8c6b-ff093e4c3ecc" />

