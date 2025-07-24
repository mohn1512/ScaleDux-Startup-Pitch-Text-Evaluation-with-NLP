
# Startup Pitch Text Evaluation with NLP

##  Overview

**Task 2: Startup Pitch Text Evaluation with NLP** focuses on extracting and preprocessing text from startup pitch deck PDFs using a hybrid pipeline for downstream natural language processing (NLP) tasks.

The pipeline:
- Uses **pdfplumber** for direct text extraction.
- Falls back to **EasyOCR** when text extraction fails (e.g., scanned images).
- Cleans and preprocesses extracted text to remove OCR artifacts, normalize formatting, and structure the content.

This project processes pitch decks from companies like **Airbnb**, **Facebook**, **DoorDash**, and **Uber**.

---

##  Repository Structure

```

ScaleDux-Startup-Pitch-Text-Evaluation-with-NLP/
├── notebook/
│   └── Startup\_PitchTextEvaluation\_WithNLP.ipynb
├── output/
│   ├── chart/
│   │   ├── word\_cloud.png
│   │   ├── radar\_chart.png
│   │   ├── heatmap.png
│   │   └── bar\_chart.png
│   ├── extracted\_decks/
│   └── result.csv
├── ScaleDux\_Startup Pitch Text Evaluation with NLP-MohanRajMurugesan.pdf
└── README.md

````


## Prerequisites

- Python **3.8+**
- A virtual environment (recommended)
- **Poppler** installed for `pdf2image` (PDF-to-image conversion)

### Poppler Installation

- **macOS**:  
  ```bash
  brew install poppler ```

* **Ubuntu**:

  ```bash
  sudo apt-get install poppler-utils
  ```

* **Windows**:
  Download and add [Poppler for Windows](http://blog.alivate.com.au/poppler-windows/) to your PATH.

---


## 3. Install Required Dependencies

Ensure `poppler` is installed (see above). Then run:


```bash
pip install pdf2image pillow easyocr pdfplumber numpy
```

---


##  Author

**Mohan Raj Murugesan**
Contributed to ScaleDux - Startup Text Pitch Evaluation with NLP project.




