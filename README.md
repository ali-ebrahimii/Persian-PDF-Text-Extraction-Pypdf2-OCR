# Persian PDF Text Extraction (PyPDF2 + OCR)

This project provides a simple and effective pipeline for **extracting Persian (Farsi) text from PDF files**, using a combination of:

* **PyPDF2** for normal text-based PDFs
* **OCR** (Tesseract or other engines) for scanned or image-based PDFs
* **Post-processing & cleaning** to fix common Persian character issues
* **Structured CSV export** for downstream NLP or dataset creation

It is ideal for research, academic projects, dataset preparation, or preprocessing Persian books and articles.

---

## 📂 Repository Contents

```
Persian-PDF-Text-Extraction-Pypdf2-OCR/
│
├── PDF_Text_Extraction.ipynb   # Main Jupyter notebook for extraction pipeline
├── pdf_extraction_summary.csv   # Output summary of extracted text
└── README.md                    # Documentation
```

---

## 🚀 Features

* Supports **Farsi/Persian PDFs**
* Automatic detection:
  ✓ text-based PDF → extract with PyPDF2
  ✓ scanned PDF → extract via OCR
* Cleans and normalizes Persian text (ی / ك / ‌ / …)
* Exports results to a clean CSV file
* Works well for books, articles, and scientific PDFs

---

## ▶️ Usage

1. Open the main notebook:

```
PDF_Text_Extraction.ipynb
```

2. Set the input directory containing PDFs

3. Run all cells to extract:

   * Raw text
   * Cleaned text
   * OCR results (if needed)

4. Final output will be saved into:

```
pdf_extraction_summary.csv
```

---

## 📦 Requirements

Install basic dependencies:

```bash
pip install pypdf2 pytesseract pandas
```

If using OCR, install Tesseract:

### macOS (Homebrew)

```bash
brew install tesseract
```

### Linux (Ubuntu)

```bash
sudo apt-get install tesseract-ocr
```
