# SAVIS Web Application

This repository contains the web application frontend and backend services for **SAVIS (Audio-Visual Instance Segmentation)**. The application allows users to sign in, upload videos and audio, run sounding object segmentation, and view interactive visual result predictions.

---

## 🏗️ Project Layout & Dependencies

The backend service in this repository depends on the core **SAVIS** modeling repository. They must be placed as sibling directories:

```
savis-project/
├── savis/         (Core model repository, e.g. from https://github.com/Sayyam-Akram/savis)
└── savis_web/     (Web app repository, this directory)
```

---

## 🚀 Getting Started

### 1. Backend Setup (Flask)

The Flask backend requires PyTorch, Detectron2, and the SAVIS core environment. Ensure you have followed the installation guide in the core repository to set up the `savis` conda environment.

Activate your conda environment and start the Flask backend:
```bash
# Activate core SAVIS environment
conda activate savis

# Navigate to backend directory and start server
cd backend
python app.py
```

The backend server will launch and listen at `http://127.0.0.1:5000/`.

> [!NOTE]
> If running on a CPU-only host without a GPU or trained checkpoints, you can run in mock mode by setting the `MOCK_INFERENCE` environment variable:
> ```bash
> MOCK_INFERENCE=1 python app.py
> ```

### 2. Frontend Setup (React + Vite)

Go to the frontend directory, install dependencies, and start the development server:
```bash
cd frontend
npm install
npm run dev
```

The frontend application will run locally at `http://localhost:5173/`.

---

## 🛡️ License

This project is licensed under the MIT License.
