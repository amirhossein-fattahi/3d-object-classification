# 🧊 3D Object Classification — ModelNet10 & ModelNet40

[![Python](https://img.shields.io/badge/python-3.9+-blue.svg)]()
[![Jupyter](https://img.shields.io/badge/jupyter-notebooks-orange.svg)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## 👥 Authors
- Amirhossein Fattahi
- Reza Sarkhosh

---

## 📂 Project Overview

This project explores **3D object classification** using both **voxel-based CNNs** and **PointNet** architectures, trained on the **ModelNet10** and **ModelNet40** datasets.  
We further investigate the impact of **orientation labels** (12 discrete azimuth angles) on classification performance.

---

## 📁 Project Structure

- **1️⃣ Model Training Notebooks**  
  Train models on preprocessed `.npy` datasets (voxel or point cloud).

  | Notebook | Description |
  |----------|-------------|
  | `MN10_Our_Model.ipynb` | Voxel-based model on ModelNet10, no orientation |
  | `MN10_PointNet.ipynb` | PointNet on ModelNet10, no orientation |
  | `MN40_Our_Model.ipynb` | Voxel-based model on ModelNet40, no orientation |
  | `MN40_PointNet.ipynb` | PointNet on ModelNet40, no orientation |
  | `OriMN10_Our_Model.ipynb` | Voxel-based model on ModelNet10, with orientation |
  | `OriMN10_PointNet.ipynb` | PointNet on ModelNet10, with orientation |
  | `OriMN40_PointNet.ipynb` | PointNet on ModelNet40, with orientation |

  > ⚠️ These notebooks load `.npy` datasets from Google Drive due to GitHub size limits.

- **2️⃣ Preprocessing Notebooks (run separately)**  
  Generate voxelized grids and point clouds from ModelNet data.

  | Notebook | Description |
  |----------|-------------|
  | `PointCloud-Part-MN40.ipynb` | Point cloud generation for ModelNet40 |
  | `PointCloud-Part-OrientationMN40.ipynb` | Point cloud generation for ModelNet40 w/ orientation |
  | `Voxelization-Part-MN10.ipynb` | Voxelization for ModelNet10, no orientation |
  | `Voxelization-Part-MN40.ipynb` | Voxelization for ModelNet40, no orientation |
  | `Voxelization-Part-OrientationMN10.ipynb` | Voxelization for ModelNet10, w/ orientation |

  > 📦 Output: `.npy` files used as input to training notebooks.

---

## 🚀 Quick Start

Clone this repository:
```bash
git clone https://github.com/amirhossein-fattahi/3d-object-classification.git
cd 3d-object-classification
