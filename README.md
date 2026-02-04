#  Clothing Segmentation & Color Recognition (YOLO + SAM)

This repository contains **Phase 1** of a larger Virtual Wardrobe & Outfit Recommendation project.  
The goal of this phase is to:

- Detect people and clothing regions in images
- Segment garments using Meta's Segment Anything Model (SAM)
- Extract dominant clothing colors from segmented regions
- Visualize segmentation masks and color swatches

This module forms the **foundation for garment understanding** in the Virtual Wardrobe pipeline.

---

## 🔍 Features

- ✅ Person detection using YOLOv8  
- ✅ Precise garment segmentation using Segment Anything (SAM)  
- ✅ Mask overlay visualization  
- ✅ Dominant color extraction from segmented clothing  
- ✅ Output visualization (original image, mask overlay, color patch)  
- ✅ JSON export of extracted attributes  

---

## 🧠 Tech Stack

- Python 3.10+
- Ultralytics YOLOv8
- Segment Anything (SAM – ViT-B)
- OpenCV
- NumPy
- Matplotlib
- PyTorch

---

## 📁 Project Structure

```bash
phase1/
│
├── data/
│   ├── raw_images/        # Input images
│   └── masks/             # Segmentation masks (generated)
│
├── models/
│   └── sam/
│       └── sam_vit_b_01ec64.pth
│
├── outputs/
│   ├── json/              # Extracted attributes (color, etc.)
│   └── visualizations/   # Mask overlays and color swatches
│
├── scripts/
│   ├── yolo_detect.py
│   ├── sam_segment.py
│   ├── color_extraction.py
│   └── visualize_results.py
│
├── inspect_model.py
├── requirements.txt
└── README.md
