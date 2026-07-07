# 🌟 Interactive 3D Particle Hand System (Selfie-Mirrored)

An advanced, production-ready frontend experience combining **Three.js** and **MediaPipe Hands** to create an interactive 3D particle system controlled entirely by hand gestures via webcam. 

The system features real-time fluid morphing between complex mathematical shapes, interactive physics pushes, and a perfected, zero-latency horizontal mirroring algorithm that matches your physical movements exactly in Selfie Mode.

---

## ✨ Features

* **⚡ Real-Time Gesture Tracking:** Powered by MediaPipe Hands for high-fidelity, low-latency joint mapping.
* **📐 Advanced Math Morphing:** Seamlessly lerps $18,000$ particles between a 3D Heart, Star, and Sphere based on the number of extended fingers.
* **🪞 Perfected Mirror Physics:** Fully resolves the classic horizontal mirroring issue. Moving your physical hand to the right shifts the particle manipulation and system rotation perfectly to the right side of the screen.
* **💥 Dynamic Force Fields:** Switch to a single-finger gesture to dynamically push particles away with custom proximity vector equations.
* **🔍 Pinch-to-Scale:** Dynamic scaling of the 3D system based on the distance between the thumb and index finger (Right hand).

---

## 🎮 Gesture Guides

Control the particle system using the following finger configurations:

| Extended Fingers | Action / Shape | Description |
| :--- | :--- | :--- |
| **1 Finger (Index)** | 💥 Push Mode | Dynamically push and repel particles |
| **2 Fingers** | ⭐ Star Shape | Morph particles into a 3D star structure |
| **3 Fingers** | 🌐 Sphere Shape | Morph particles into a symmetrical sphere |
| **0 or 4+ Fingers** | ♥️ Heart Shape | Morph particles into a 3D pulsing heart (Default) |

---

## 🛠️ Architecture & Tech Stack

The architecture is entirely self-contained within a single, highly-optimized HTML5 file requiring zero build steps or npm installations.

* **Rendering Engine:** Three.js (r128) using optimized `THREE.BufferGeometry` and `THREE.PointsMaterial` with Additive Blending.
* **Machine Learning:** MediaPipe Hands & Camera Utilities hosted via reliable jsDelivr CDNs.
* **Performance Optimization:** Pixel ratios are dynamically capped at $\min(\text{devicePixelRatio}, 2)$ to guarantee stable 60 FPS performance across modern desktop and mobile devices.

---

## 🚀 Getting Started

Since the project uses absolute client-side CDNs and vanilla modern JavaScript, you don't need any complex setups.