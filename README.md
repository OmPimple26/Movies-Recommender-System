# Movies-Recommender-System
An AI-powered movie recommendation app that suggests the top 5 similar films based on your favorite title. Uses TMDB API for posters and a similarity model for accurate results. Simple, fast, and interactive—discover your next favorite movie instantly! 🚀🎥

---

## 🚀 Features

🧠 Content-based filtering using cosine similarity

🎨 Beautiful Streamlit UI

🖼️ Fetches HD movie posters using TMDB API

⚡ Fast predictions using precomputed similarity matrix

🔒 Secure API key storage using st.secrets

☁️ Fully deployable on Streamlit Cloud

---

## 📁 Project Structure
```
.gitattributes
.gitignore
app.py
LICENSE
movie_dict.pkl
movies.pkl
README.md
requirements.txt
similarity.pkl
```

---

## 🛠️ Installation & Setup (Local)
1️⃣ Clone the Repository
```
git clone https://github.com/OmPimple26/Movies-Recommender-System.git
cd Movies-Recommender-System
```

2️⃣ Install Dependencies
```
pip install -r requirements.txt
```

3️⃣ Add your TMDB API Key

Create a file:

```
.streamlit/secrets.toml
```


Add:

```
TMDB_API_KEY = "your_api_key_here"
```

4️⃣ Run the App
```
streamlit run app.py
```

---

## 🌐 Deployment on Streamlit Cloud
1️⃣ Push your code to GitHub

Streamlit Cloud fetches the files directly.

2️⃣ Add Secrets

In Streamlit Cloud → App → Settings → Secrets:

```
TMDB_API_KEY = "your_api_key_here"
```

3️⃣ Deploy

Choose:

Python version: 3.13

Main file: app.py

Requirements file: requirements.txt

---

## 🔑 TMDB API Usage

Inside app.py, we securely fetch the API key:

```
api_key = st.secrets["TMDB_API_KEY"]
```


Poster fetching:

```
url = f"https://api.themoviedb.org/3/movie/{movie_id}?api_key={api_key}&language=en-US"
```

---

## 📸 Screenshots

<img width="1920" height="853" alt="Movies Recommender System Image" src="https://github.com/user-attachments/assets/031f3189-bf32-4b13-995d-7f2f42bb96f6" />

---

## 🔧 Technologies Used

Python

Streamlit

NumPy

Pandas

Scikit-learn

TMDB API

Pickle for pre-trained model files

---

## 🧑‍💻 Author

Om Pimple
If you like this project, ⭐ the repository!

---

## 📄 License

This project is open-source and available under the MIT License.
✅ requirements.txt
✅ Improved UI version of app.py
✅ GitHub tags + short repo description
