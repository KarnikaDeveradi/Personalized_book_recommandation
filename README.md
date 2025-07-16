# 📚 Book Recommendation System

This is a content-based **Book Recommendation Web Application** developed using **Python**, **Flask**, and **Machine Learning techniques**. The system suggests books similar to the one entered by the user by analyzing book features and similarity scores derived from collaborative filtering. It features a user-friendly interface where users can explore popular books and get recommendations instantly.

---

## 🚀 Key Features

- ✅ Displays the **most popular books** with titles, authors, ratings, votes, and cover images  
- ✅ **Suggests similar books** based on user input using cosine similarity  
- ✅ Clean and responsive **Flask-based UI** using HTML and Jinja templates  
- ✅ Loads preprocessed datasets for **fast performance** with no recomputation needed  
- ✅ Lightweight and easy to run locally on any machine  

---

## 🧠 How the Recommendation Works

The recommendation engine is based on **collaborative filtering** using a precomputed **cosine similarity matrix**:

1. A user enters the name of a book.
2. The system looks up the index of this book in the pivot table (`pt.pkl`).
3. It retrieves similarity scores from `similarity_scores.pkl` for that index.
4. Top 5 most similar books are selected.
5. Book details (title, author, image) are fetched from `books.pkl` and displayed.

All heavy computations are done offline and stored in `.pkl` files for efficient access.

---

## 🗂 Project Directory Structure

```

book-recommendation/
├── app.py                      # Flask application file
├── templates/
│   ├── index.html              # Homepage - displays popular books
│   └── recommend.html          # Recommendations page
├── static/                     # (Optional) CSS or image assets
├── popular.pkl                 # Top-rated/popular books data
├── pt.pkl                      # Pivot table for book-user matrix
├── books.pkl                   # Book metadata (title, author, image)
├── similarity\_scores.pkl       # Precomputed cosine similarity matrix
└── README.md                   # Project documentation

````

---

## 🛠 Tech Stack

| Component       | Technology       |
|----------------|------------------|
| Language        | Python           |
| Framework       | Flask            |
| Data Handling   | pandas, numpy    |
| Frontend        | HTML, Jinja2     |
| Data Storage    | Pickle (`.pkl`)  |
| Recommendation  | Cosine Similarity |

---

## 💻 How to Run the Project

### 📦 Prerequisites

Make sure you have Python installed, and install required libraries:

```bash
pip install flask pandas numpy
````

### 🚀 Steps to Run Locally

1. **Clone the repository**

```bash
git clone https://github.com/yourusername/book-recommendation.git
cd book-recommendation
```

2. **Ensure the following `.pkl` files are present:**

* `popular.pkl`
* `pt.pkl`
* `books.pkl`
* `similarity_scores.pkl`

3. **Run the Flask app**

```bash
python app.py
```

4. **Open your browser** and go to:

```
http://127.0.0.1:5000
```

---

## 📝 Sample Usage

* Go to the homepage to see **trending books**.
* Click on **“Get Recommendations”** or visit `/recommend`.
* Enter a book title (e.g., `The Hobbit` or `Harry Potter`).
* Get a list of **5 similar books** with author names and cover images.

---

## 🔮 Future Enhancements

* 🔍 Add auto-complete search for better user input
* 📚 Include genre or category filters
* 🌐 Deploy on Render, Heroku, or AWS
* 🔐 Implement user login and personalized recommendations
* 📱 Make the frontend mobile-responsive with better UI/UX

---

## 🙏 Acknowledgements

* Dataset: [Book-Crossing Dataset (Kaggle)](https://www.kaggle.com/datasets/arashnic/book-recommendation-dataset)
* Inspired by collaborative filtering-based systems and recommender engines

---

## 📬 Contact

**Developer:** Your Name
📧 Email: [your.email@example.com](mailto:your.email@example.com)
🔗 GitHub: [@yourusername](https://github.com/yourusername)

---

## ⭐ Like this project?

If you found this project helpful or interesting, please give it a ⭐ on GitHub – it really helps support my work and reach more developers!

```

---

✅ Paste the copied content into your `README.md` file on GitHub.  
Let me know if you’d like help generating `requirements.txt` or want deployment steps next!
```

