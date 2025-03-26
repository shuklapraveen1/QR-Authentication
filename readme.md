# QR Code Authentication: Detecting Original vs. Counterfeit Prints

## Introduction
This project focuses on classifying QR codes as either **original (first prints)** or **counterfeit (second prints)** using machine learning and deep learning techniques. The dataset contains QR codes with embedded copy detection patterns (CDPs) to help distinguish between original and counterfeit prints.

## Features
- **Data Preprocessing**: Converts images to grayscale, resizes to 128x128, and normalizes pixel values.
- **Feature Engineering**:
  - Sobel Edge Detection
  - Histogram of Oriented Gradients (HOG)
- **Traditional ML Model**: Random Forest Classifier
- **Deep Learning Model**: Convolutional Neural Network (CNN)
- **Performance Metrics**: Accuracy, Precision, Recall, F1-score
- **Misclassification Analysis**

## Installation
### 1. Clone the Repository
```bash
git clone https://github.com/shuklapraveen1/QR-Authentication.git
cd qr-authentication
```
### 2. Install Dependencies
```bash
pip install -r requirements.txt
```
### 3. Prepare Dataset
Place QR code images into separate folders:
```
/dataset/
    ├── first_print/
    ├── second_print/
```
### 4. Run the Script
```bash
python qr_authentication.py
```

## Results
| Model | Accuracy | Precision | Recall | F1-score |
|--------|----------|-----------|--------|----------|
| Random Forest | 100% | 1.00 | 1.00 | 1.00 |
| CNN | 100% | 1.00 | 1.00 | 1.00 |

## Deployment Considerations
- Model should handle **different scanning conditions**.
- **Optimization required** for real-time inference.
- Future work: Deploy using **Flask/FastAPI**.

## License
This project is open-source under the MIT License.

