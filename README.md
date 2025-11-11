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
### Environment Setup
<pre> ```bash # Create and activate virtual environment python -m venv venv # For macOS/Linux source venv/bin/activate # For Windows venv\Scripts\activate ``` </pre>






