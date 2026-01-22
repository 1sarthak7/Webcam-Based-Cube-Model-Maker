# VOXEL
Webcam-Based 3D Voxel / Cube Model Maker

A gesture-controlled 3D voxel modeling system that allows users to create, place, delete, and manipulate 3D cubes in real time using only a webcam and hand gestures no mouse, keyboard, or controller required.

This project explores the future of human–computer interaction (HCI) by combining computer vision, gesture recognition, and real-time 3D rendering.

🚀 Project Overview

Traditional 3D modeling tools require complex interfaces and precise input devices, making them difficult to use for beginners, students, and accessibility-focused applications.

This project introduces an intuitive, touch-free 3D modeling approach where:
A webcam captures live video
Hand gestures are detected using computer vision
Gestures are mapped to 3D actions
Cubes (voxels) are dynamically placed in a 3D space

The result is a natural, immersive, and interactive 3D creation experience.


🎯 Key Features

📷 Real-time webcam input

✋ Hand gesture recognition
🧱 3D voxel (cube) creation & deletion
🔄 Scene rotation & navigation using gestures

🎯 Grid-snapped cube placement
🖥️ Live 3D rendering
📊 On-screen HUD (gesture, mode, FPS)

🧠 Gesture Controls
Gesture
Action
Pinch (thumb + index)
Place cube
Fist
Delete cube
Open palm
Rotate 3D scene
Index finger point
Move 3D cursor
Two-finger pinch
Depth / scale control
(Gestures are temporally filtered to reduce false triggers.)

🏗️ System Architecture

The system is modular and scalable:
Copy code

├── camera_thread.py     # Webcam capture & preprocessing
├── gesture_engine.py   # Gesture detection & logic
├── voxel_engine.py     # 3D grid & cube management
├── renderer.py         # Real-time 3D rendering (OpenGL)
├── ui.py               # HUD and visual feedback
├── main.py             # Application entry point

Each module is independent, making the project easy to extend or refactor.

🛠️ Tech Stack
Python 3
OpenCV – real-time video processing
MediaPipe – hand landmark & gesture detection
PyOpenGL / Pygame – 3D rendering
NumPy – mathematical operations
PyQt (optional) – UI & overlays

⚙️ Installation & Setup

1️⃣ Clone the repository

Copy code
Bash

git clone https://github.com/your-username/webcam-3d-voxel-maker.git
cd webcam-3d-voxel-maker

2️⃣ Create a virtual environment (recommended)
Copy code

Bash
python3 -m venv .venv
source .venv/bin/activate  # macOS / Linux

3️⃣ Install dependencies
Copy code
Bash
pip install opencv-python mediapipe numpy pygame PyOpenGL PyQt6

4️⃣ Run the application
Copy code
Bash
python main.py

🧪 Use Cases

🎓 Education – teaching 3D geometry and spatial thinking

🏗️ Architecture & design – quick concept modeling

🧠 HCI research – gesture-based interaction systems

♿ Accessibility tools – touch-free modeling interfaces

🕶️ AR / VR foundations – natural input pipelines

🌟 Novelty & Innovation
Touch-free 3D modeling using only a webcam

Gesture-based interaction instead of traditional UI

Combines computer vision + graphics + interaction design

Scalable toward AR/VR and mixed-reality systems

This concept has strong potential for patenting and startup exploration, especially in the domain of natural user interfaces.

📌 Future Enhancements
Undo / redo gesture support
Save & export 3D models (OBJ / STL)
AR overlay using depth estimation
Multi-hand collaboration
Voice + gesture hybrid controls
ML-based gesture customization

👨‍💻 Author
Sarthak Bhopale
Engineering Student | Computer Vision & Interactive Systems

📌 Built as a semester-level Design Thinking & Technical Innovation project

📜 License
This project is open sourced and 
Feel free to use, modify, and build upon it.
