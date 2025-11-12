# 3D Reconstruction and Bundle Adjustment

This project focuses on **3D image registration and reconstruction** using the **Buddha dataset**. It implements a full pipeline for computing **fundamental matrices**, **triangulating 3D points**, and performing **bundle adjustment** using tools such as **GTSAM**, **OpenCV**, or **SciPy**.  

The project continues from previous assignments on image registration, extending the approach to **Structure-from-Motion (SfM)** in 3D.

---

## 📸 Overview

The goal of this assignment is to reconstruct a 3D scene from multiple 2D images.  
Key steps include:

1. **Feature Detection & Matching**  
   - Detect feature keypoints (e.g., SIFT, ORB, or SuperPoint).  
   - Match features across image pairs.  

2. **Fundamental and Essential Matrix Estimation**  
   - Compute **F** (Fundamental Matrix) between image pairs using RANSAC.  
   - Recover **E** (Essential Matrix) and camera pose.  

3. **Triangulation**  
   - Use corresponding 2D points to reconstruct 3D points in space.  
   - Visualize sparse 3D point cloud.  

4. **Bundle Adjustment**  
   - Refine both camera poses and 3D points to minimize reprojection error.  
   - Implemented using **GTSAM** or other optimization frameworks.  

---

## 🧠 Dataset

**Buddha Dataset:**  
[Google Drive Link](https://drive.google.com/drive/folders/1PFrGwrTAVvezGXptI4Jgm3MiMIshoa_b?usp=sharing)

Each image captures the Buddha statue from different viewpoints, enabling multi-view reconstruction.

---

## ⚙️ Implementation Details

- Language: **Python 3**
- Libraries Used:
  - `OpenCV` – feature detection, matching, and triangulation
  - `NumPy` – numerical operations
  - `Matplotlib` – visualization
  - `GTSAM` / `SciPy` – bundle adjustment optimization
- Optional Tools for Comparison:
  - [COLMAP](https://colmap.github.io/)
  - [OpenSfM](https://github.com/mapillary/OpenSfM)
  - [Agisoft Metashape](https://www.agisoft.com/)

---


## 📊 Results

- Computed pairwise **Fundamental Matrices** with robust RANSAC filtering.  
- Triangulated sparse **3D point cloud**.  
- Optimized camera poses and structure using **bundle adjustment**.  
- Visualized reconstructed scene in 3D.

---

## 🧾 References

- [Princeton SfMedu (MATLAB)](https://github.com/jianxiongxiao/SFMedu)  
- [COLMAP Documentation](https://colmap.github.io/)  
- [OpenSfM](https://github.com/mapillary/OpenSfM)  
- [GTSAM Library](https://gtsam.org/)

---

