# 📄 Medical Report OCR using YOLO & Tesseract

## An end-to-end Custom Optical Character Recognition (OCR) system
to extract structured data from medical lab reports using YOLO-based
object detection and Tesseract OCR.

## 🚀 Project Overview

Medical reports are often scanned or image-based, making data extraction manual and error-prone.
This project automates the process by:
- Detecting text regions using YOLO
- Cropping detected regions
- Applying image preprocessing
- Extracting text using Tesseract OCR
- Saving results in CSV / JSON format

## 🏗️ System Architecture
```bash
    Input Image
        ↓
    YOLO Text Detection
        ↓
    Bounding Box Cropping
        ↓
    Image Preprocessing
        ↓
    Tesseract OCR
        ↓
    Structured Output (CSV / JSON)
```

Dataset

## Custom medical lab report images
- YOLO-format annotations
- Train / Validation / Test split
- Stored on Google Drive / Cloud Storage

## 🤖 Model Details
YOLOv3 / YOLOv8 for text region detection Custom-trained on medical report layouts

#### Classes include:
- Patient Info
- Test Headers
- Numeric Results
- Reference Ranges
- Date / Time
- Footer Notes

### Image Preprocessing
- To improve OCR accuracy:
- Grayscale conversion
- CLAHE contrast enhancement
- Noise removal
- Thresholding & normalization

### 🛠️ Technologies Used
- 🐍 Python
- 📸 OpenCV
- 🔍 Tesseract OCR
- 🤖 YOLO (Object Detection)
- ☁️ Google Colab / AWS (Optional)
- 📊 Pandas, NumPy

### ▶️ How to Run
```bash
    pip install -r requirements.txt
    python Custom_OCR.py --image sample.jpg
```

### 📈 Output
- Extracted text saved as:
    * ocr_results.csv
    * ocr_results.json
- Detailed processing logs
- Structured medical data ready for analysis

### 💰 Cost Estimation
- Google Colab (Free Tier): $0
- Google Drive: 15GB Free
- AWS (Optional): Pay-as-you-go

### 🔮 Future Improvements
- NLP-based data validation
- LayoutLM / Transformer OCR
- Web dashboard (Streamlit)
- Hospital EMR integration

### 👨‍💻 Author
Mr. Aniket Tayade
AI Engineer | Data Scientist
📧 Open to opportunities & collaborations