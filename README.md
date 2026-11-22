# llm-ps52-ADT23SOCB1199


# 💊 Prescription Reader – Problem Statement 52

## Project Overview
Prescription Reader is an AI-powered application that extracts medicine names, dosages, timings, and duration from handwritten prescription images and typed text. It converts the extracted information into a structured medicine schedule.

## Technologies Used
- Python
- Google Colab
- Gradio
- Pytesseract OCR
- OpenCV
- Google Gemini Flash API
- Pandas
- Pillow

## Features
- Upload handwritten prescription images (JPG/PNG).
- Enter prescription text manually.
- Extract text using Pytesseract OCR.
- Preprocess images using OpenCV.
- Organize medicine details using Gemini Flash.
- Display medicine name, dosage, timings, duration, and notes.
- Flag unclear information for verification.
- Download the medicine schedule as CSV.

## Project Workflow

**Image Input:**
Prescription Image → OpenCV → Pytesseract OCR → Gemini Flash → Structured JSON → Pandas Table → CSV Download

**Text Input:**
Typed Text → Gemini Flash → Structured JSON → Pandas Table → CSV Download

## Installation

Install dependencies:

```bash
pip install -r requirements.txt
```

Install Tesseract OCR:

```bash
sudo apt-get install tesseract-ocr
```

## How to Run
1. Open the notebook in Google Colab.
2. Install the required dependencies.
3. Add `GEMINI_API_KEY` to Google Colab Secrets.
4. Run all notebook cells.
5. Open the Gradio application.
6. Upload a prescription image or enter text.
7. View and download the extracted medicine schedule.

## Limitations
- OCR accuracy depends on handwriting and image quality.
- Medicine names and dosages may be misinterpreted.
- Unclear details require manual verification.

## Disclaimer
This project is an educational prescription transcription aid and does not provide medical advice. All extracted information must be verified against the original prescription by a qualified pharmacist or prescriber before use.

## Project Information
- **Category:** AI / Healthcare
- **Language:** Python
- **Platform:** Google Colab
