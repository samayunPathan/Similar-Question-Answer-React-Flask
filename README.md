# Question-Answering System

This project implements a question-answering system with a React frontend and a Flask backend. It uses cosine similarity to find the most similar question in a PostgreSQL database and returns the corresponding answer.

## Features

- **React frontend** for user interaction
- **Flask backend API** for processing requests
- **PostgreSQL database** for storing question-answer pairs
- **Natural Language Processing (NLP)** techniques for text preprocessing
- **Cosine similarity** for finding the most relevant answer

## Backend (Flask)

The Flask backend provides an API endpoint that receives questions from the frontend, processes them, and returns the most similar question-answer pair from the database.

### Key Components

- Flask application setup
- SQLAlchemy for database operations
- NLTK for text preprocessing (tokenization, stop word removal, lemmatization)
- TfidfVectorizer for text vectorization
- Cosine similarity calculation

### API Endpoint

- **POST /api**: Accepts a question and returns the most similar question-answer pair

## Frontend (React)

The React frontend provides a user interface for submitting questions and displaying answers.

## Database

- **PostgreSQL** database with a QA table storing question-answer pairs.

## Setup and Installation

1. Clone the repository

 ```bash
git clone https://github.com/samayunPathan/Similar-Question-Answer-React-Flask.git
```
```bash
Similar-Question-Answer-React-Flask
```
cd 
3. Set up the PostgreSQL database
4. Install backend dependencies:
    ```bash
    pip install flask flask_sqlalchemy psycopg2 nltk scikit-learn
    ```
5. Install frontend dependencies:
    ```bash
    npm install
    ```
6. Run the Flask backend:
    ```bash
    python app.py
    ```
7. Run the React frontend:
    ```bash
    npm start
    ```

## Usage

1. Enter a question in the frontend interface
2. The question is sent to the Flask backend
3. The backend processes the question, finds the most similar question in the database
4. The corresponding answer is returned and displayed in the frontend

## Future Improvements

- Implement user authentication
- Add functionality to add new question-answer pairs
- Improve similarity matching with more advanced NLP techniques
