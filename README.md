# 🫀 Embryonic Medaka Fish Cardiac Analysis

## 📋 Project Overview
This project implements a comprehensive cardiac analysis pipeline for embryonic medaka fish, developed as part of the Biomedical and Health AI Scientist (KTP Associate) Interview Task for Hurdle.bio. The system processes time series TIFF images to detect cardiac regions and estimate heart rate using classical computer vision and signal processing techniques.

## 🎯 Objectives
Temporal Analysis: Process 130 sequential frames with precise timing information

Embryo Detection: Automatically identify and isolate the embryonic region using Hough Circle Transform

Cardiac Signal Extraction: Detect heart regions and track intensity variations over time

Heart Rate Estimation: Calculate cardiac frequency using Fourier analysis and peak detection

Comprehensive Visualization: Generate detailed plots and output files for analysis validation


## 🛠 Technical Implementation

### Core Methodology

| Component | Technique | Purpose |
|-----------|-----------|---------|
| **Preprocessing** | Median Blur, CLAHE Enhancement | Noise reduction and contrast improvement |
| **Embryo Detection** | Hough Circle Transform | Automatic circular region identification |
| **Temporal Analysis** | Frame interval calculation | Precise timing for heart rate estimation |
| **Signal Processing** | FFT, Peak Detection, Butterworth Filtering | Cardiac frequency extraction |

### Key Features
Automated Processing: Handles 130 frames with temporal metadata extraction

Robust Detection: Identifies embryonic regions with 233-pixel radius accuracy

Signal Analysis: Implements detrending, filtering, and frequency domain analysis

Comprehensive Outputs: Generates frames, signals, and analysis reports

## 📁 Project Structure

Bio_Medical/
├── Heart_Detection.ipynb          # Main analysis notebook
├── rawTiff/                       # Input TIFF image sequence (130 frames)
├── outputs/                       # Generated analysis outputs
│   ├── frames/                    # Processed frame visualizations
│   └── signals/                   # Extracted cardiac signals
├── requirements.txt               # Python dependencies
└── README.md                      # Project documentation

## ⚙️ Installation & Setup

### 1. Environment Setup
```bash
# Create and activate virtual environment
python -m venv venv
# For macOS/Linux
source venv/bin/activate  
# For Windows
venv\Scripts\activate
````
### 2. Install Dependencies
```bash
pip install -r requirements.txt
````
### Required Packages:
```bash
opencv-python==4.8.1.78
numpy==1.24.3
scipy==1.10.1
matplotlib==3.7.1
scikit-image==0.21.0
pandas==2.0.3
tqdm==4.65.0
````
### 3. Data Preparation
Place TIFF image sequence in rawTiff/ directory with naming convention: *--T[timestamp]*.tif

## 🚀 Usage
```bash
jupyter notebook Heart_Detection.ipynb
````

## Pipeline Steps
### 1. Frame Loading & Temporal Analysis

Loads 130 sequential frames

Extracts timing from filenames (T-values)

Calculates frame rate (12.89 fps) and total duration (10.01 seconds)

### 2. Embryo Detection

Applies median blur and CLAHE enhancement

Uses Hough Circle Transform for automatic detection

Identifies embryo center at (1138, 986) with 233px radius

### 3. Cardiac Analysis

Processes cardiac region across all frames

Extracts intensity signals for heart rate calculation

Implements signal filtering and peak detection

### 4. Output Generation

Saves processed frames and signals

Generates comprehensive visualizations

Produces heart rate estimates and analysis metrics







