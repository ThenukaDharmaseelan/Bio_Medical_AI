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


