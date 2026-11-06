# OCR Invoice Reader

Python FastAPI service that extracts structured fields from invoice images using Tesseract OCR.

Designed for accounts-payable style demos: vendor, dates, invoice numbers, and totals parsed into editable structured output.

## Stack

- **Backend:** Python 3.11+, FastAPI, Uvicorn
- **OCR / vision:** Tesseract (pytesseract), Pillow
- **Frontend (optional demo UI):** React + Vite

## Features

- Image upload for invoice parsing
- Field extraction into structured JSON
- Sample invoice asset for local testing
- Works offline once Tesseract is installed

## Quick start

```bash
cd backend
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
# system package also required: tesseract-ocr
uvicorn main:app --reload --port 8004
```

API docs: http://localhost:8004/docs

```bash
cd frontend
npm install
npm run dev
```

## Author

Pooja Sharma — [Pooja101117](https://github.com/Pooja101117)
