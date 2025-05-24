# 🩺 Breast Cancer Decision Support System (SSD)

This is a decision support system designed to assist in early detection and risk evaluation of breast cancer. It combines a web-based interface, a CNN model trained on mammography images, and statistical models (Gail / Tyrer-Cuzick) to provide an integrated evaluation for clinicians or patients.

---

## 🚀 Features
- ✅ Web form for patient risk factors input
- ✅ Upload and process mammography images
- ✅ Custom-built Convolutional Neural Network (CNN)
- ✅ Statistical risk evaluation (Gail model)
- ✅ Grad-CAM heatmap visualization
- ✅ PDF report generation and email delivery
- ✅ Modular FastAPI backend + SQLite/PostgreSQL DB

---

## 📦 Project Structure

```
breast-cancer-decision-support-system-ssd/
├── main.py                     # entry point (FastAPI app)
├── requirements.txt            # all dependencies
├── README.md                   # main documentation

├── src/                        # core source code
│   ├── ui/                     # web interface
│   │   ├── templates/          # HTML (Jinja2)
│   │   └── static/             # CSS, JS, frontend assets
│   │
│   ├── ai/                     # AI models (CNN, Grad-CAM)
│   │   ├── cnn_model.py        # model architecture + training
│   │   └── predict.py          # inference logic
│   │
│   ├── backend/                # FastAPI endpoints (routes)
│   │   └── api.py
│   │
│   ├── db/                     # SQLAlchemy ORM models
│   │   └── models.py
│   │
│   └── utils/                  # helper utilities
│       ├── report.py           # PDF generation
│       └── gradcam.py          # heatmap visualization
│
├── risk_models/                # statistical risk models
│   ├── gail/                   # Gail model
│   │   └── gail_score.py
│   ├── tyrer_cuzick/           # Tyrer-Cuzick model
│   │   └── tyrer_score.py
│   └── __init__.py

├── models/                     # saved AI models (.h5)
├── data/                       # mammography images and input data
├── tests/                      # automated tests
├── docs/                       # extended documentation
└── SSD.code-workspace          # VS Code workspace config
```

---

## ⚙️ Local Installation

### Clone & install dependencies:
```bash
git clone https://github.com/YOUR_USERNAME/Breast-Cancer-Decision-Support-System-SSD.git
cd Breast-Cancer-Decision-Support-System-SSD
pip install -r requirements.txt
```

### Run the server:
```bash
uvicorn main:app --reload
```
Open: [http://127.0.0.1:8000](http://127.0.0.1:8000)

---

## 📊 Dataset Resources

- CBIS-DDSM: https://wiki.cancerimagingarchive.net/display/Public/CBIS-DDSM
- MIAS: https://www.kaggle.com/datasets/aryashah2k/mias-mammography

---

## 🧠 Technologies Used

- FastAPI (backend REST API)
- Jinja2 + Bootstrap (frontend UI)
- TensorFlow (CNN)
- OpenCV (image preprocessing)
- SQLAlchemy (ORM)
- FPDF (PDF generation)
- Matplotlib (Grad-CAM visualization)

---

## 📌 Future Improvements

- User authentication (doctors/patients)
- Cloud deployment (Render / Railway)
- Dockerization for easy portability
- Upload & view DICOM format directly
- Integration with HL7 / FHIR for hospital systems

---

## 📄 License

This project is open-source and available under the MIT License.
