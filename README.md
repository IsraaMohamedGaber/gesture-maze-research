# Gesture Maze - Model Serving (FastAPI)

This branch provides the production-ready backend to serve the trained hand gesture model via an API.

## 🚀 API Features

- Serves the selected model (`best_model.pkl`) via FastAPI
- Accepts landmark data from frontend
- Returns gesture prediction as JSON

## 🔁 API Endpoint

**POST** `/predict/`

### 🔸 Request Body:

{
  "landmarks": [0.1, 0.2, 0.3, ..., 0.7]  # 63 float values (21 points × x, y, z)
}

### 🔸 Response:

{
  "gesture": "left"
}

### 📁 Structure

gesture-maze-prod/
├── app/
│   └── main.py              # FastAPI app
├── models/
│   └── best_model.pkl       # Copied from research repo
├── requirements.txt
└── README.md                # This file


### ▶️ Run the API Locally

Install dependencies:

pip install -r requirements.txt
