Startup Pitch Text Evaluation with NLP
Overview
This project, Task 2: Startup Pitch Text Evaluation with NLP, focuses on extracting and preprocessing text from startup pitch deck PDFs for natural language processing (NLP) analysis. The pipeline extracts text from PDFs using a hybrid approach combining pdfplumber for direct text extraction and EasyOCR for image-based text extraction when direct extraction fails. The extracted text is then cleaned and preprocessed to remove OCR artifacts, normalize formatting, and structure the content for downstream NLP tasks.
The repository includes scripts to:

Extract text from PDF pitch decks.
Clean and preprocess the extracted text to remove OCR errors and normalize formatting.
Save the cleaned text in a structured format for further analysis.

The project processes multiple pitch deck files (e.g., Airbnb, Facebook, DoorDash, Uber).
Repository Structure
ScaleDux-Startup-Pitch-Text-Evaluation-with-NLP/
├── notebook/
│   └── Startup_PitchTextEvaluation_WithNLP.ipynb                    
├── output/
│   ├── chart/   
│   |   ├── word_cloud.png
│   |   ├── radar_chart.png
│   |   ├── heatmap.png
│   |   └── bar_chart.png
|   ├── extracted_decks/               
│   └── result.csv
├── ScaleDux_Startup Pitch Text Evaluation with NLP-MohanRajMurugesan.pdf                        
└── README.md

Prerequisites

Python 3.8+
A virtual environment (recommended)
Poppler installed for pdf2image (required for PDF-to-image conversion)
On macOS: brew install poppler
On Ubuntu: sudo apt-get install poppler-utils
On Windows: Install via Poppler binaries



Installation

Clone the repository:
git clone https://github.com/your-username/pitchdeck-nlp-analysis.git
cd pitchdeck-nlp-analysis


Set up a virtual environment:
python3 -m venv myenv
source myenv/bin/activate  # On Windows: myenv\Scripts\activate


Install dependencies:
Ensure Poppler is installed (see Prerequisites).


Dependencies
The requirements.txt includes:
pdf2image
pillow
easyocr
pdfplumber
numpy

Install them using:
pip install pdf2image pillow easyocr pdfplumber numpy
