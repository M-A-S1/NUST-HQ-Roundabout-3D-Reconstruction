# NUST HQ Roundabout 3D Reconstruction

This project demonstrates the 3D reconstruction of the NUST Pakistan HQ Library and Auditorium using COLMAP.

## 🎥 Dense Point Cloud Demonstration

![NUST 3D Reconstruction](Demo.gif)

## 📸 Input Data

- A collection of images capturing various angles of the NUST HQ, Library and Auditorium.

## 🛠️ Reconstruction Pipeline

1. **Feature Extraction**: Detect and extract features from input images.
2. **Feature Matching**: Match features across images to establish correspondences.
3. **Sparse Reconstruction**: Perform Structure-from-Motion (SfM) to estimate camera poses and generate a sparse point cloud.
4. **Dense Reconstruction**: Use Multi-View Stereo (MVS) to generate a dense point cloud.
5. **Meshing**: Create 3D meshes from the dense point cloud using Poisson or Delaunay meshing.

## 📁 Folder Structure

- `images/`: Contains the input images.
- `sparse/`: Contains the sparse reconstruction files.
- `dense/`: Contains the dense reconstruction files and meshes.

## 🚀 Getting Started

1. Clone the repository:

```bash
   git clone https://github.com/yourusername/NUST-3D-Reconstruction.git
   cd NUST-3D-Reconstruction
```
2. Place your input images in the images/ folder.

3. Run COLMAP and then follow automatic 3D reconstruction steps

## Results 

![NUST 3D Reconstruction](path_to_your_gif.gif)
