# 🩺 Breast Cancer SSD - Local Version

Aplicație locală FastAPI cu UI Web, CNN, și calcul statistic pentru evaluarea riscului de cancer de sân.

## 📦 Structură
- `src/ui` – Interfață Web (formulare + upload imagini)
- `src/ai` – Rețea neuronală CNN custom
- `src/risk_model` – Calcul model Gail / Tyrer-Cuzick
- `src/db` – Bază de date cu SQLAlchemy
- `src/backend` – API FastAPI
- `src/utils` – Generare PDF, procesare imagini

## ▶️ Rulare locală
```bash
pip install -r requirements.txt
uvicorn main:app --reload
```
Accesează aplicația la `http://127.0.0.1:8000`
