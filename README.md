# SkyVision

SkyVision: Multi-scale Aerial Object Detection and Segmentation.

## Team

- Huynh Quoc Viet
- Le Nguyen Gia Hung
- Vo Tan Phat

## Course

DAT301m — Applied Machine Learning

## Problem Statement

Aerial imagery introduces unique computer vision challenges: the top-down perspective makes objects appear with limited contextual cues, many targets are arbitrarily oriented, and object sizes vary drastically from very small to large across scenes. SkyVision addresses these challenges by building a detection and segmentation pipeline for densely distributed aerial objects using YOLOv8-OBB and SAHI on the DOTA-v2.0 dataset.

## Installation

1. Create and activate a Python virtual environment:

   ```bash
   python -m venv .venv
   source .venv/bin/activate
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Basic Usage

1. Place DOTA-v2.0 patches in `data/`.
2. Implement data processing and training logic in `src/`.
3. Train baseline model:

   ```bash
   python src/train_baseline.py
   ```

4. Evaluate model:

   ```bash
   python src/evaluate.py
   ```

5. Launch Gradio app:

   ```bash
   python app/app.py
   ```
