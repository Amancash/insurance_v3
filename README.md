# InsureIQ v3 🏥

AI-powered Health Insurance Risk Predictor with Explainable AI, Wearable Sync, and Medical Report Parsing.

## Features
- 🔮 **Risk Prediction** — Predicts Low / Medium / High insurance risk
- 🧠 **Explainable AI** — SHAP-based explanation of every prediction
- 💊 **Medical Report Parser** — Upload blood test PDF/image, auto-extracts health metrics
- ⌚ **Wearable Sync** — Google Fit / Apple Health lifestyle discount
- 📊 **Social Benchmarking** — Compare your risk with users in your city & age group
- 🎯 **What-If Optimizer** — Shows exactly what lifestyle changes reduce your premium

## Tech Stack
- **Backend** — FastAPI + Scikit-learn + SHAP
- **Frontend** — Streamlit
- **Database** — SQLite
- **AI** — Google Gemini API (report parsing)

## Setup

### 1. Install dependencies
pip install -r requirements.txt

### 2. Add API Key
Create a `.env` file:
GOOGLE_API_KEY=your_key_here

Get free key from: aistudio.google.com

### 3. Run Backend
uvicorn app:app --reload

### 4. Run Frontend
streamlit run frontend.py

## Project Structure
- `app.py` — FastAPI backend & all endpoints
- `frontend.py` — Streamlit UI
- `database.py` — SQLite auth & prediction history
- `explainer.py` — SHAP explainability engine
- `report_parser.py` — Gemini AI medical report parser
- `wearable.py` — Wearable data sync & discount engine
- `model.pkl` — Trained ML model (not included, run training script)