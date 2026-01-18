# Gesture-Based Music Recommendation Setup

## README.md
```
# Gesture-Based Music Recommendation System

This project recommends music based on real-time hand gestures using a webcam.
It uses MediaPipe for hand tracking, OpenCV for computer vision, and PyTorch for
computing gesture-based embeddings for song recommendations.

---

## Environment Requirements

To run this notebook reliably from top to bottom without errors, we recommend:

- Python 3.10 (Important!)
- pip (latest)
- OS: Windows / Linux / Mac

---

## Dependencies

All required Python packages are included in `requirements.txt`:
'''

numpy==1.26.4
opencv-contrib-python==4.12.0.88
mediapipe==0.10.8
torch==2.5.1
torchvision==0.20.1
torchaudio==2.5.1
scikit-learn==1.7.2
pandas==2.2.3
matplotlib==3.10.7

'''

------------------------------------------------------------------

## Setup Instructions

### Step 1: Create a local virtual environment
```bash

# Linux / Mac
python3.10 -m venv venv
source venv/bin/activate

# Windows
python -m venv venv
venv\Scripts\activate

```

### Step 2: Install dependencies
```bash

pip install --upgrade pip
pip install -r requirements.txt

```

### Step 3: Open Jupyter Notebook
```bash

jupyter notebook

```

### Step 4: Run "workflow.ipynb"

- Run **all cells** from top to bottom
- The notebook is tested with **Python 3.10** and the package versions in `requirements.txt`
- **Important:** Do not change MediaPipe version, otherwise `NameError` may occur.

---

## Optional: Colab

- If running on Colab, the notebook requires **Python ≥3.12**, so the original MediaPipe 0.10.8 is **not available**.
- Either:
  1. Rewrite imports to use `mediapipe>=0.10.31` and `mp.solutions.*` API, or
  2. Use a local Python 3.10 environment for full compatibility. --> "Prefered"

---

## Notes

- This notebook is designed to run **top-to-bottom without errors** in the recommended environment.
- Hand gesture recognition and song recommendation modules are fully integrated.
- For any issues, please check your Python version and package versions.
```

