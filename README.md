# 3D Object Classification Project - ModelNet10 & ModelNet40

### Authors:
- Amirhossein Fattahi 2109245
- Reza Sarkhosh 2109663
---

## 📁 Project Structure

The project is structured into two main parts:
1. Model Training Notebooks
2. Preprocessing Notebooks (Voxelization / PointCloud generation)

---

## 1️⃣ Model Training Notebooks

These notebooks load the processed datasets and train different models based on data type (voxel or point cloud), dataset (ModelNet10/ModelNet40), and orientation task (enabled/disabled).

| Notebook | Description |
|----------|-------------|
| MN10_Our_Model.ipynb | Voxel-based model on ModelNet10, without orientation |
| MN10_PointNet.ipynb | PointNet model on ModelNet10, without orientation |
| MN40_our_model.ipynb | Voxel-based model on ModelNet40, without orientation |
| MN40_PointNet.ipynb | PointNet model on ModelNet40, without orientation |
| OriMN10_Our_Model.ipynb | Voxel-based model on ModelNet10, with orientation |
| OriMN10_PointNet.ipynb | PointNet model on ModelNet10, with orientation |
| OriMN40_PointNet.ipynb | PointNet model on ModelNet40, with orientation |

> 🧠 Note: These notebooks load preprocessed datasets (saved as .npy files) from Google Drive due to size limitations.

---

## 2️⃣ Preprocessing Notebooks (Run on another machine)

Due to hardware limitations, the voxelization and point cloud generation steps were performed on a separate machine. These notebooks generate the .npy datasets used above.

| Notebook | Description |
|----------|-------------|
| PointCloud-Part-MN40.ipynb | Point cloud generation for ModelNet40 (no orientation) |
| PointCloud-Part-OrientationMN40.ipynb | Point cloud generation for ModelNet40 with orientation labels |
| Voxelization-Part-MN10.ipynb | Voxelization for ModelNet10, no orientation |
| Voxelization-Part-MN40.ipynb | Voxelization for ModelNet40, no orientation |
| Voxelization-Part-OrientationMN10.ipynb | Voxelization for ModelNet10, with orientation |

> 📦 These notebooks output .npy files for point clouds and voxel grids, which are later used in training.

---

## 🧩 Notes

- All final datasets were uploaded to Google Drive and mounted in Colab for training.
- Training notebooks automatically load the required .npy files from the shared Drive path.
- Orientation labels are based on 12 discrete azimuth angles.
---