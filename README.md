# 🏛️ NUST 3D Reconstruction – Library & Jinnah Auditorium

This project showcases a full 3D reconstruction of the NUST Pakistan HQ, Library and Jinnah Auditorium using **COLMAP**. It includes both **sparse** and **dense** reconstructions, mesh generation, and **metric scaling** using real-world measurements.

---

## 🎬 Dense 3D Reconstruction Demo

![Dense Reconstruction Demo](demo.gif)

*Above: Rotating view of the dense 3D point cloud generated with COLMAP.*

---

## 📏 Metric Reconstruction Using Real-World Scaling

To convert the 3D reconstruction into **real-world metric scale**, I followed this process:

### 1. 📐 Real-World Measurement (Google Maps)

Used Google Maps to measure the **length of Jinnah Auditorium**’s exterior wall.

![Google Maps Measurement](1.png)

*Measured length: ~50 meters*

---

### 2. 🧱 Model Measurement (COLMAP/Viewer)

Measured the **same wall** in the unscaled mesh using a 3D viewer.

![Model Measurement](2.png)

*Measured length in mesh units: ~5 units*

---

### 3. ⚖️ Scaling the Model

Calculated the scale factor:

Scale Factor = Real Length / mesh Length = 41.22 / 3.41 = 12.1

Applied this factor to rescale the model, resulting in a **metric-accurate 3D reconstruction**.

---

## 🗂️ Project Structure

NUST-3D-Reconstruction/
├── images/ # Input video frames
├── sparse/ # Sparse reconstruction (COLMAP)
├── dense/ # Dense reconstruction and mesh outputs
├── assets/
│ ├── dense_demo.gif # GIF demo of 3D reconstruction
│ ├── google_maps_measurement.jpg
│ └── model_measurement.jpg
├── README.md
└── LICENSE
