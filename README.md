# 🦅 H.A.W.K. — Hybrid Adaptive Waypoint Knowledge for Multi-Domain UAV Navigation

An AI-powered autonomous drone navigation system using **Computer Vision** and **NLP** techniques for intelligent object detection, adaptive decision-making, and multi-domain waypoint navigation.

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![YOLOv8](https://img.shields.io/badge/YOLOv8-FF6B35?style=for-the-badge)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![Status](https://img.shields.io/badge/Status-Published%20Paper-success?style=for-the-badge)

---

## 📄 Published Research

> **Paper Title:** H.A.W.K. : Hybrid Adaptive Waypoint Knowledge for Multi-Domain UAV Navigation
> **Published:** April 2026
> **Domain:** Artificial Intelligence / Computer Vision / NLP
> **Author:** Tharun Nalamasu

---

## 📌 About the Project

Modern UAVs (Unmanned Aerial Vehicles) struggle to navigate autonomously across **multiple environments** — urban, rural, indoor, and outdoor — without human intervention. **H.A.W.K.** solves this by combining Computer Vision and NLP to enable a drone to **see**, **understand**, and **decide** its path intelligently in real time.

> The system adapts its navigation strategy based on the domain it detects, making it truly multi-environment capable.

---

## ✨ Features

- 🎯 **Autonomous Navigation** — Drone navigates without human control using AI-generated waypoints
- 👁️ **Real-time Object Detection** — YOLOv8 detects obstacles, landmarks, and targets live
- 🧠 **Intelligent Decision-Making** — NLP module interprets mission commands and environmental context
- 🌍 **Multi-Domain Adaptability** — Works across urban, rural, indoor, and outdoor environments
- 📍 **Waypoint Knowledge System** — Dynamically generates and updates navigation waypoints
- ⚡ **Adaptive Response** — Adjusts flight path in real time based on detected obstacles
- 🔄 **Hybrid AI Architecture** — Combines vision + language understanding for robust navigation

---

## 🛠️ Tech Stack

| Component | Technology |
|-----------|------------|
| Language | Python |
| Object Detection | YOLOv8 |
| Deep Learning Framework | PyTorch |
| Computer Vision | OpenCV |
| NLP | Python NLP Libraries |
| Navigation Logic | Custom Waypoint Engine |
| Simulation *(if applicable)* | *(add your simulator — e.g. Gazebo, AirSim)* |

---

## 🧠 System Architecture

```
Mission Input (Text Command / Coordinates)
              │
              ▼
     ┌─────────────────────┐
     │   NLP Interpreter   │  ← Parses mission goals & domain context
     └────────┬────────────┘
              │
              ▼
     ┌─────────────────────┐
     │  Waypoint Knowledge │  ← Generates adaptive waypoint path
     │      Engine         │
     └────────┬────────────┘
              │
              ▼
     ┌─────────────────────┐
     │   YOLOv8 Vision     │  ← Real-time obstacle & object detection
     │      Module         │     via OpenCV frame capture
     └────────┬────────────┘
              │
              ▼
     ┌─────────────────────┐
     │  Decision Engine    │  ← Decides: continue / reroute / hover
     │  (PyTorch Model)    │
     └────────┬────────────┘
              │
              ▼
     UAV Executes Navigation Command
```

---

## 📊 Model Performance

| Metric | Score |
|--------|-------|
| Object Detection Accuracy | *(add your value)* |
| Navigation Success Rate | *(add your value)* |
| Obstacle Avoidance Rate | *(add your value)* |
| Average Waypoint Deviation | *(add your value)* |

---

## 📁 Project Structure

```
hawk-uav-navigation/
├── detection/
│   ├── yolo_detector.py          # YOLOv8 object detection module
│   └── object_classes.yaml       # Target object definitions
├── navigation/
│   ├── waypoint_engine.py        # Adaptive waypoint generation
│   ├── path_planner.py           # Route planning logic
│   └── domain_classifier.py     # Multi-domain environment detection
├── nlp/
│   ├── command_parser.py         # NLP mission command interpreter
│   └── context_analyzer.py      # Environmental context understanding
├── decision/
│   └── decision_engine.py        # PyTorch-based decision model
├── simulation/
│   └── sim_runner.py             # Simulation environment runner
├── utils/
│   ├── camera.py                 # OpenCV camera/frame utilities
│   └── logger.py                 # Flight log utilities
├── models/
│   └── hawk_model.pt             # Trained PyTorch model weights
├── requirements.txt
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites
```
Python >= 3.9
CUDA-compatible GPU (recommended for real-time inference)
Webcam or drone camera feed
```

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/tharunalamasu/hawk-uav-navigation.git
cd hawk-uav-navigation

# 2. Create virtual environment
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Download YOLOv8 weights
python -c "from ultralytics import YOLO; YOLO('yolov8n.pt')"

# 5. Run the navigation system
python navigation/waypoint_engine.py
```

### Requirements (`requirements.txt`)
```
ultralytics
torch
torchvision
opencv-python
numpy
pandas
nltk
matplotlib
```

---

## 📸 Screenshots / Demo

> *Add simulation screenshots, detection outputs, or demo video link here*

| Object Detection | Waypoint Map | Navigation Output |
|-----------------|--------------|-------------------|
| ![detection](#) | ![waypoint](#) | ![nav](#) |

---

## 🔬 Research Highlights

- **Hybrid AI** — First-of-its-kind combination of vision + NLP for UAV navigation
- **YOLOv8 Integration** — State-of-the-art real-time object detection at high FPS
- **Multi-domain** — Single system handles urban roads, forests, indoor corridors
- **Adaptive Waypoints** — Navigation path updates dynamically as environment changes
- **NLP Commands** — Drone understands natural language mission instructions
- **PyTorch Backbone** — Custom deep learning model for intelligent flight decisions

---

## 🌐 Research Paper

🔗 [Read the Published Paper](#) *(add your publication link here)*

---

## 🙋‍♂️ Author

**Tharun Nalamasu**
📧 tharunnalamasu@gmail.com
🔗 [LinkedIn](https://linkedin.com/in/tharunnalamasu) · [GitHub](https://github.com/tharunalamasu)

---

## 📄 License

This project is for research and educational purposes.

---

<div align="center">

⭐ <i>Star this repo if you find it interesting — it supports open research!</i>

</div>
