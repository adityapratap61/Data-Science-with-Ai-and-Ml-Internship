# Project 9: Text Recognizer

This project explores optical character recognition (OCR) using EasyOCR and PyTesseract. It includes sample images, notebooks for experimentation, and a local Tesseract installer.

## Features

- OCR experiments with EasyOCR.
- OCR experiments with PyTesseract.
- Sample image inputs: `img1.jpeg`, `img2.jpeg`, and `img3.jpeg`.
- Notebook-based testing workflow.
- Included Windows Tesseract installer for local setup.

## Project Structure

```text
Project_9_Text_recognizer/
+-- README.md
+-- requirements.txt
+-- ocr_testing.ipynb
+-- pytesseract_testing.ipynb
+-- img1.jpeg
+-- img2.jpeg
+-- img3.jpeg
+-- tesseract_downloaded/
    +-- tesseract-ocr-w64-setup-5.4.0.20240606.exe
```

## Setup

```bash
cd Project/Project_9_Text_recognizer
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
```

For PyTesseract, install the Tesseract OCR engine separately. On Windows, you can use the installer included in `tesseract_downloaded/`.

## How to Use

Open the notebooks and run the cells:

```bash
jupyter notebook
```

Use:

- `ocr_testing.ipynb` for EasyOCR experiments.
- `pytesseract_testing.ipynb` for PyTesseract experiments.

## Notes

- EasyOCR can download model files the first time it runs.
- PyTesseract requires the Tesseract executable to be installed and available on your system path, or configured explicitly in the notebook.
