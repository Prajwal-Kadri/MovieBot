# MovieBot

MovieBot is a lightweight Flask web application that demonstrates session-based login and simple user profile storage using SQLite with SQLAlchemy.

## Features

- Login flow with session persistence
- User profile page to save/update an email address
- Flash messages for login/logout and session states
- SQLite-backed user records
- Page to view stored users

## Tech Stack

- Python
- Flask
- Flask-SQLAlchemy
- SQLite
- Bootstrap 4 (CDN)

## Project Structure

- `app.py` — Flask app, routes, and database model
- `base.html` — Shared layout and navigation
- `index.html` — Home page
- `login.html` — Login form
- `user.html` — User email update form
- `view.html` — User list page

## Getting Started

1. Clone the repository.
2. Create and activate a Python virtual environment.
3. Install dependencies:
   - `pip install flask flask-sqlalchemy flask-sqlalchemy-session`
4. Run the app:
   - `python app.py`
5. Open the local URL shown in the terminal (default: `http://127.0.0.1:5000`).

## Usage

1. Go to `/login` and submit a username.
2. Go to `/user` to add or update the email for that username.
3. Visit `/view` to see all stored users.
4. Use `/logout` to clear the current session.

## Notes

- The app uses a local SQLite database file: `users.sqlite3`.
- Session lifetime is set to 5 minutes in `app.py`.
