# Movie Recommendation System – Content Based Filtering

A fully–functional Movie Recommendation System built using Machine Learning + NLP, deployed as a clean Streamlit web application.
The system recommends movies based on similarity of plot, genres, keywords, cast, and director using text vectorization + cosine similarity.

📸 Demo Screenshots

(Add your screenshots here — replace the placeholder image links after uploading images to GitHub)

Homepage

Recommendations Output

🎯 Project Overview

This project analyzes movie metadata from the TMDB 5000 dataset and creates a unified “tag” representation for each movie by combining:

Movie overview

Genres

Keywords

Cast

Director

These tags are processed using Bag of Words (CountVectorizer) and similarity is computed using Cosine Similarity.

The web interface (Streamlit) allows users to select any movie and instantly receive the top recommended similar movies — optionally with posters.

🧠 Key Features

✔ Content-Based Recommendation using textual similarity
✔ Combines multiple metadata fields into one unified tag
✔ NLP preprocessing (tokenization, stemming, cleaning)
✔ Vectorization using CountVectorizer (max_features=5000)
✔ Distance calculation via Cosine Similarity
✔ Real-time recommendations via the Streamlit UI
✔ Ability to show movie posters if poster_path is available
✔ Clean + interactive web interface

🏗 Tech Stack
Component	Technology
Backend Processing	Python, Pandas, NumPy
NLP	NLTK (PorterStemmer)
Machine Learning	CountVectorizer, Cosine Similarity
Frontend Web App	Streamlit
Dataset	TMDB 5000 Movies + Credits
📂 Project Structure
Movie-Recommendation-System/
│── README.md                   # Project documentation 
│── requirements.txt            # Dependencies
│── app.py                      # Streamlit main application
│── tmdb_5000_movies.csv.zip    # Dataset (optional)
│── tmdb_5000_credits.csv.zip   # Dataset (optional)
│── assets/                     # Screenshots for README
│   ├── homepage.png
│   └── recommend.png

⚙️ How the Model Works (Conceptual)

Load TMDB dataset

Extract important fields:

Overview

Genres

Keywords

Cast

Crew (Director)

Normalize + Preprocess text:

Convert JSON-like fields

Remove spaces

Tokenize

Apply stemming (PorterStemmer)

Build “tags” column by merging all fields

Vectorize tags using CountVectorizer

Compute cosine similarity matrix

For input movie → return top K most similar movies

▶️ How to Run This Project (Locally or Codespaces)
1. Install dependencies
pip install -r requirements.txt

2. Run the application
streamlit run app.py

3. The app opens at
http://localhost:8501

🌐 Deploying to Hugging Face Spaces

This project can be deployed easily:

Create a Space (Streamlit template)

Upload app.py and requirements.txt

Add dataset or download script

Space auto-builds and provides a public URL

(Add your Hugging Face link here once deployed)

🚧 Future Improvements

🔹 Use TF-IDF Vectorizer for better text representation
🔹 Introduce Neural Embeddings (Sentence Transformers)
🔹 Add trailer previews and additional metadata
🔹 Create hybrid recommender (content-based + collaborative filtering)
🔹 Host backend as an API + frontend separately

🙌 Author

Mohammad Ali ZaidiMovie Recommendation System – Content Based Filtering

A fully–functional Movie Recommendation System built using Machine Learning + NLP, deployed as a clean Streamlit web application.
The system recommends movies based on similarity of plot, genres, keywords, cast, and director using text vectorization + cosine similarity.

📸 Demo Screenshots

(Add your screenshots here — replace the placeholder image links after uploading images to GitHub)

Homepage

Recommendations Output

🎯 Project Overview

This project analyzes movie metadata from the TMDB 5000 dataset and creates a unified “tag” representation for each movie by combining:

Movie overview

Genres

Keywords

Cast

Director

These tags are processed using Bag of Words (CountVectorizer) and similarity is computed using Cosine Similarity.

The web interface (Streamlit) allows users to select any movie and instantly receive the top recommended similar movies — optionally with posters.

🧠 Key Features

✔ Content-Based Recommendation using textual similarity
✔ Combines multiple metadata fields into one unified tag
✔ NLP preprocessing (tokenization, stemming, cleaning)
✔ Vectorization using CountVectorizer (max_features=5000)
✔ Distance calculation via Cosine Similarity
✔ Real-time recommendations via the Streamlit UI
✔ Ability to show movie posters if poster_path is available
✔ Clean + interactive web interface

🏗 Tech Stack
Component	Technology
Backend Processing	Python, Pandas, NumPy
NLP	NLTK (PorterStemmer)
Machine Learning	CountVectorizer, Cosine Similarity
Frontend Web App	Streamlit
Dataset	TMDB 5000 Movies + Credits
📂 Project Structure
Movie-Recommendation-System/
│── app.py                      # Streamlit main application
│── README.md                   # Project documentation
│── requirements.txt            # Dependencies
│── tmdb_5000_movies.csv.zip    # Dataset (optional)
│── tmdb_5000_credits.csv.zip   # Dataset (optional)
│── assets/                     # Screenshots for README
│   ├── homepage.png
│   └── recommend.png

⚙️ How the Model Works (Conceptual)

Load TMDB dataset

Extract important fields:

Overview

Genres

Keywords

Cast

Crew (Director)

Normalize + Preprocess text:

Convert JSON-like fields

Remove spaces

Tokenize

Apply stemming (PorterStemmer)

Build “tags” column by merging all fields

Vectorize tags using CountVectorizer

Compute cosine similarity matrix

For input movie → return top K most similar movies

▶️ How to Run This Project (Locally or Codespaces)
1. Install dependencies
pip install -r requirements.txt

2. Run the application
streamlit run app.py

3. The app opens at
http://localhost:8501

🌐 Deploying to Hugging Face Spaces

This project can be deployed easily:

Create a Space (Streamlit template)

Upload app.py and requirements.txt

Add dataset or download script

Space auto-builds and provides a public URL

(Add your Hugging Face link here once deployed)

🚧 Future Improvements

🔹 Use TF-IDF Vectorizer for better text representation
🔹 Introduce Neural Embeddings (Sentence Transformers)
🔹 Add trailer previews and additional metadata
🔹 Create hybrid recommender (content-based + collaborative filtering)
🔹 Host backend as an API + frontend separately

🙌 Author
Mohammad Ali Zaidi

🙌 Author

Mohammad Ali Zaidi
