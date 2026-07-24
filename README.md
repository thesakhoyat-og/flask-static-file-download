# Flask Static File Download App

This is a simple Flask project that demonstrates how to serve static files using Python Flask.

The app displays a clean Bootstrap-based webpage where users can download a ZIP file from the `static` folder.

## Features

- Simple Flask web server
- HTML template rendering using `render_template`
- Static file serving
- Downloadable ZIP file
- Bootstrap-based responsive design
- Beginner-friendly project structure

## Technologies Used

- Python
- Flask
- HTML
- Bootstrap
- Static Files

## Project Structure

FLASK_SERVING_STATIC/
│
├── main.py
├── README.md
├── templates/
│   └── index.html
└── static/
    └── 1.zip

## How It Works

The Flask app creates a local web server using Python.

When the user visits the homepage, Flask runs the route function and renders the `index.html` file from the `templates` folder.

The `index.html` page contains a download button. When the user clicks the button, the ZIP file stored inside the `static` folder is downloaded.

## Main Flask Code

from flask import Flask, render_template

app = Flask(__name__)

@app.route("/")
def home():
    return render_template("index.html")

app.run(debug=True, port=8000)

## How to Run the Project

### 1. Install Flask

pip install flask

### 2. Run the app

python main.py

### 3. Open in browser

http://127.0.0.1:8000/

## What I Learned

Through this project, I learned:

- How Flask works with Python
- How to create routes in Flask
- How to render HTML templates
- How to serve static files
- How to create a download link for a ZIP file
- How Bootstrap can improve webpage design
- The difference between the `templates` folder and the `static` folder

## Author

Sakhoyat Hossain Siam