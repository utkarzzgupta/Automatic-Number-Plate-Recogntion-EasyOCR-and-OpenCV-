# Automatic-Number-Plate-Recogntion-EasyOCR-and-OpenCV-
# 🚘 Automatic Number Plate Recognition (ANPR) using OpenCV & EasyOCR

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat-square&logo=python)
![OpenCV](https://img.shields.io/badge/OpenCV-Edge--Detection-orange?style=flat-square&logo=opencv)
![EasyOCR](https://img.shields.io/badge/EasyOCR-Text--Recognition-green?style=flat-square)

## 📌 Project Overview

This project demonstrates a simple and effective **Automatic Number Plate Recognition (ANPR)** system using:
- **OpenCV** for image preprocessing and contour detection
- **EasyOCR** for extracting text from the detected license plate

It is capable of reading text from license plates in real-world car images using computer vision and deep learning-based OCR techniques.

---

## ✨ Key Features

- Read and preprocess images using OpenCV
- Detect license plate region using edge detection & contour approximation
- Extract the plate area and mask the rest
- Apply EasyOCR to extract text from the cropped image
- Overlay the detected number plate text back onto the original image

---

## 🛠️ Tech Stack

- Python 3.10+
- OpenCV
- EasyOCR
- NumPy
- Matplotlib
- imutils

---

## 📷 Workflow Steps

1. **Read image & convert to grayscale**
2. **Apply bilateral filtering** to remove noise while preserving edges
3. **Detect edges** using Canny
4. **Find contours** and approximate them to locate rectangular plates
5. **Mask the plate** and extract it from the original image
6. **Crop the region of interest**
7. **Run EasyOCR** on the cropped image to read text
8. **Display result** with bounding box and recognized text

---

## 💡 Sample Output

```python
[([[18, 0], [298, 0], [298, 70], [18, 70]], 'CCC44l', 0.18)]
