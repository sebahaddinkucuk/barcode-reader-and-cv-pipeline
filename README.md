# 📷 Advanced Barcode Detection and Reading System

This project is a two-stage system that detects and extracts barcode data using computer vision and optical character recognition (OCR). It includes a user-friendly desktop graphical interface (GUI) and a research notebook demonstrating the step-by-step algorithmic filtering processes.

## 🚀 Project Contents

### 1. Desktop GUI Application (`main.py`)
- Graphical User Interface developed using **Tkinter**.
- High-speed barcode decoding via the **Pyzbar** library.
- Real-time barcode detection and bounding box rendering from a PC webcam.
- Support for reading barcodes from uploaded static images.

### 2. Image Processing and OCR Pipeline (`goruntu.ipynb`)
A computer vision algorithm built from scratch for scenarios where barcodes are difficult to detect. This notebook processes the sample image `barkodddd(1).png` step-by-step:
- **Sobel Operator:** Detects vertical edges on the X-axis to highlight barcode lines.
- **Morphological Operations:** Uses `cv2.morphologyEx` to close gaps and isolate the Region of Interest (ROI) containing the barcode.
- **Tesseract OCR:** Extracts the numerical digits located at the bottom of the detected region using `pytesseract`.
- **Matplotlib:** Visualizes the entire pipeline, including grayscale conversion, thresholding, and morphological filtering steps.

## 🛠️ Technologies Used
- **Language:** Python
- **Computer Vision:** OpenCV, Numpy, PIL (Pillow)
- **Barcode & OCR:** Pyzbar, Pytesseract
- **Data Visualization:** Matplotlib
- **GUI:** Tkinter

## 📦 Installation and Usage
1. Clone the repository to your local machine.
2. Install the required libraries:
   `pip install -r requirements.txt`
3. Ensure that Tesseract OCR is installed on your system.
4. To launch the desktop interface:
   `python main.py`
5. To explore the computer vision pipeline, open and run `goruntu.ipynb` via Jupyter Notebook or VS Code to see how it processes the sample image.
