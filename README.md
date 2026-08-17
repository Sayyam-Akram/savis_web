# SAVIS Web Application

This repository contains the web application frontend and backend services for **SAVIS (Audio-Visual Instance Segmentation)**. The application allows users to sign in, upload videos and audio, run sounding object segmentation, and view interactive visual result predictions.

---

## 🏗️ Project Structure

The project is split into two main directories:

*   **`frontend/`**: A React + Vite web application styled with TailwindCSS/CSS, using Firebase for user authentication.
*   **`backend/`**: A Flask-based REST API service that manages user databases (SQLite), handles file uploads, and serves segmentation visualization results.

---

## 🚀 Getting Started

### 1. Backend Setup (Flask)
Go to the backend directory and set up the environment:
```bash
cd backend
python3 -m venv venv
source venv/bin/activate
pip install Flask flask-cors opencv-python Pillow numpy
```
Start the backend server:
```bash
python app.py
```
The server will start at `http://127.0.0.1:5000/`.

### 2. Frontend Setup (React + Vite)
Go to the frontend directory and install dependencies:
```bash
cd ../frontend
npm install
```
Start the development server:
```bash
npm run dev
```
The application will run locally at `http://localhost:5173/`.

---

## 🛡️ License

This project is licensed under the MIT License.
