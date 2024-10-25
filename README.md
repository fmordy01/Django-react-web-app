# NoteKeeper

**NoteKeeper** is a full-stack web application for managing personal notes. Built with a Django backend and React frontend, this application supports user authentication via JSON Web Tokens (JWT) and provides full CRUD functionality, enabling users to create, view, update, and delete notes.

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)

## Project Overview
NoteKeeper is designed for users who want a secure, easy-to-use platform to organize and manage personal notes. Users can register for an account, log in, and have access to a personal dashboard where they can create, view, edit, and delete notes. JWT-based authentication ensures user data privacy.

## Features
- **User Registration**: Allows new users to create accounts.
- **Login**: Authenticates users and grants access to their personal notes.
- **Create Notes**: Users can add new notes.
- **Read Notes**: Users can view their saved notes.
- **Update Notes**: Allows users to modify existing notes.
- **Delete Notes**: Users can delete notes they no longer need.

## Tech Stack
- **Back-End**: Python, Django
- **Front-End**: JavaScript, React
- **Authentication**: JWT (JSON Web Tokens)
- **Database**: PostgreSQL (or other databases supported by Django)

## Installation
1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/NoteKeeper.git
   ```
2. **Navigate to the project directory**:
   ```bash
   cd NoteKeeper
   ```

### Backend Setup
3. **Set up a virtual environment**:
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```
4. **Install backend dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
5. **Set up the database**:
   - Create a PostgreSQL database and update the database configuration in the Django `settings.py` file.
   - Run migrations to create necessary tables:
     ```bash
     python manage.py migrate
     ```

6. **Run the Django server**:
   ```bash
   python manage.py runserver
   ```

### Frontend Setup
7. **Navigate to the frontend directory**:
   ```bash
   cd frontend
   ```
8. **Install frontend dependencies**:
   ```bash
   npm install
   ```
9. **Run the React development server**:
   ```bash
   npm start
   ```

10. **Access the application**: Open your browser and go to `http://localhost:3000` for the frontend, and `http://localhost:8000` for the backend.

## Usage
1. **Register/Login**: Users can register for a new account or log in with existing credentials.
2. **Create Notes**: Users can add notes from their dashboard.
3. **View Notes**: All created notes are displayed on the user dashboard.
4. **Edit Notes**: Users can update notes directly from the dashboard.
5. **Delete Notes**: Users can delete notes they no longer need.

## Project Structure
- **backend/**: Django backend for API endpoints and authentication.
- **frontend/**: React frontend for user interactions and note management.
- **static/**: Contains static files like CSS for the frontend.
- **templates/**: HTML templates for the backend.
- **tests/**: Test cases to verify functionality.
