This is a simple Flask + SQLite blog application where users can create posts and view them on the homepage.

Features
Create posts (name + content)
Display all posts
SQLite database storage
Flask backend with Jinja2 templates
Tech Stack

Python, Flask, SQLite, HTML

Project Structure
app.py → main Flask application
models.py → database functions (create/get posts)
database.db → SQLite database file
schema.sql → database schema
templates/index.html → frontend template
How to Run
Create virtual environment:
python -m venv myenv
Activate environment:
myenv\Scripts\activate
Install dependencies:
pip install flask flask-cors
Run the app:
python app.py
Open in browser:

http://127.0.0.1:5000/

Database Setup

Run this SQL in SQLite:

CREATE TABLE posts (
id INTEGER PRIMARY KEY AUTOINCREMENT,
name TEXT,
content TEXT
);

How it works
User fills the form (name + content)
Flask receives POST request
Data is saved into SQLite database
Posts are displayed on homepage
Author

Beginner Flask Project
