# DRL TurboEngine

A Deep Reinforcement Learning (DRL) engine designed to train agents on high-speed navigation tasks using custom track environments. This repository includes the full training pipeline, race environment, deployment scripts, and visualization assets.

---

## 🚀 Project Overview
DRL TurboEngine is an end‑to‑end framework built for training autonomous agents in racing-style environments. It includes:

- **Custom Race Environment** built using Python
- **Agent Training Pipeline** with reward functions, environment loops, and episode management
- **Deployment Module** to run trained policies in real-time
- **Track Assets** in both **STL** and **XML** formats
- **Testing Scripts** for validating performance

The goal of this project is to experiment with DRL in custom navigation tasks — such as racing, obstacle avoidance, and trajectory optimization.

---

## 📂 Repository Structure
```
DRL_TurboEngine/
│
├── TurboCore.py                # Core utilities and shared functions
├── TurboTraining.py            # DRL training loop
├── TurboDeploy.py              # Deployment / inference script
├── TurboRaceEnvironment.py     # Custom racing environment
├── EnvironmentTeasting.py      # Environment testing script
│
├── Tracks_STL/                 # Track models (STL format)
│   └── Track_V1/
│
├── Tracks_XML/                 # Track definitions (XML based)
│
├── assets/                     # Images and videos
│   ├── rover_image.png         # Rover model image
│   └── rover_track_demo.mp4    # Demo video of rover navigating track
│
└── README.md                   # Documentation (this file)
```

---

## 🧠 How It Works
### 1. **Environment**
The `TurboRaceEnvironment` simulates a racing-style track system. It provides:
- Observations
- Rewards
- Actions
- Episode logic

You can modify the track design, boundaries, and rules.

### 2. **Training**
`TurboTraining.py` handles:
- Agent initialization
- Episode loops
- Reward computation
- Logging & saving checkpoints

### 3. **Deployment**
`TurboDeploy.py` loads the trained model and runs it over the track for visualization or benchmarking.

---

## 📸 Demo Assets
### 🖼 Rover Image
An image showcasing the rover used during training.
```
assets/rover_image.png
```

### 🎥 Navigation Demo Video
A video of the rover navigating through the track.
```
assets/rover_track_demo.mp4
```

---

## ▶️ Getting Started
### **Clone the repository**
```
git clone https://github.com/Karthibs/DRL_TurboEngine.git
cd DRL_TurboEngine
```

### **Run Environment Test**
```
python EnvironmentTeasting.py
```

### **Start Training**
```
python TurboTraining.py
```

### **Run Deployment / Demo**
```
python TurboDeploy.py
```

---

## 🛠 Requirements
- Python 3.9+
- NumPy
- OpenCV (for video)
- PyTorch / TensorFlow (depending on your implementation)
- Matplotlib (optional for visualization)

Install dependencies:
```
pip install -r requirements.txt
```

---

## 📌 Future Improvements
- Add PPO/SAC implementations
- Add more complex tracks
- Add LiDAR‑based or camera‑based observations
- Evaluate sim‑to‑real performance

---

## 📧 Contact
Created by **Karthikeya Reddy**

If you use this repository or want to collaborate, feel free to reach out!

