# AI-Powered Alcohol Label Verification App

## Overview
This prototype assists alcohol label compliance agents by extracting text from label artwork and comparing it against application data.

## Features
- Single label upload
- Batch upload
- OCR-based text extraction
- Brand name verification
- ABV verification
- Net contents verification
- Government warning verification
- Pass / Needs Review / Fail results
- CSV export

## Tech Stack
- React
- FastAPI
- Python
- EasyOCR
- RapidFuzz
- OpenCV

## Setup Instructions

### Backend
cd backend
python -m venv venv
pip install -r requirements.txt
uvicorn main:app --reload

### Frontend
cd frontend
npm install
npm run dev

## Assumptions
- Prototype does not integrate directly with COLA.
- Uploaded files are not permanently stored.
- Bold detection for warning text is noted as a future enhancement.
- Human agents make the final compliance decision.

## Limitations
- OCR accuracy depends on image quality.
- Glare, skew, and low resolution may reduce confidence.
- Prototype focuses on common distilled spirits fields.
