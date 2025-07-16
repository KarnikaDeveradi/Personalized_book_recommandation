# 📚 Book Recommendation System

A machine learning-powered Book Recommendation Web App built with **Python**, **Flask**, and **pandas**. It suggests books similar to the one entered by the user, based on collaborative filtering and similarity scores. This project demonstrates how you can turn data science models into a functional web application.

![Book Recommendation Demo](https://your-demo-screenshot-link.com) <!-- Replace with actual screenshot or remove -->

---

## 🚀 Features

- 🔥 Shows trending books with their titles, authors, cover images, and ratings
- 📖 Recommends 5 similar books based on user input
- 🧠 Utilizes cosine similarity for recommendations
- 💻 Flask-based web interface
- 📦 Clean and modular code structure

---

## 🧠 How It Works

1. User enters the name of a book.
2. The system matches the input with the index in the pivot table (`pt.pkl`).
3. Using cosine similarity (`similarity_scores.pkl`), it finds the top 5 most similar books.
4. Metadata (title, author, image) is fetched from `books.pkl`.
5. Results are displayed on the UI (`recommend.html`).

---

## 🗂 Project Structure

book-recommendation/
├── app.py # Main Flask app
├── templates/
│ ├── index.html # Homepage showing popular books
│ └── recommend.html # Book recommendation page
├── static/ # (Optional) CSS or image files
├── popular.pkl # Data for popular books
├── pt.pkl # Pivot table of book ratings
├── books.pkl # Book metadata
├── similarity_scores.pkl # Cosine similarity matrix
└── README.md # Project documentation

yaml
Copy
Edit

---

## 🛠️ Tech Stack

- **Backend**: Flask
- **Data Processing**: pandas, numpy
- **Model**: Cosine similarity (collaborative filtering)
- **Frontend**: HTML, Jinja2 templating

---

## 💻 Getting Started

### 📦 Installation

1. **Clone the repository**

```bash
git clone https://github.com/yourusername/book-recommendation.git
cd book-recommendation
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
Run the app

bash
Copy
Edit
python app.py
Open in browser

cpp
Copy
Edit
http://127.0.0.1:5000
📂 Required Files
Ensure the following .pkl files are in your project directory:

popular.pkl

pt.pkl

books.pkl

similarity_scores.pkl

You can generate them using a Jupyter Notebook or use existing ones from your data pipeline.

📝 Example Usage
📍 On homepage: View the most popular books
🔍 On /recommend: Type a book name like "Harry Potter" to get 5 similar suggestions

📈 Future Improvements
🔍 Auto-complete/search-as-you-type feature

📅 Filter by genre, year, or author

🔐 User login system for personalized recommendations

☁️ Deploy on Heroku or Render
