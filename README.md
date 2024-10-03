# DeepEarthMY Dataset

**DeepEarthMY** is a remote sensing dataset for tropical land-cover segmentation in Malaysia. The dataset contains 4007 PNG images, each around 828 KB in size, representing different land-cover types including roads, buildings, water, forests, agriculture, barren land, and background.

![DeepEarthMY-Distribution](https://github.com/user-attachments/assets/1504bf51-ea7f-4b99-a174-d0d182cdb1a3)
![DeepEarthMY-statistics](https://github.com/user-attachments/assets/2c711a5f-2b37-4f48-9ad3-402d5de0b9fa)

## Dataset Overview

The dataset is divided into two categories:
- **Rural**
- **Urban**

Each category contains annotated images for semantic segmentation, which can be used for training and testing machine learning models to classify various land-cover types.

### File Structure

The dataset is organized as follows:

## Land-Cover Classes

The dataset provides the following land-cover classes for segmentation:
1. Roads
2. Buildings
3. Water
4. Forests
5. Agriculture
6. Barren Land
7. Background

![land-cover](https://github.com/user-attachments/assets/b3fec3f0-cc62-43f1-ba32-3bb111fdad10)

### Usage

You can use this dataset for various computer vision tasks, particularly for **semantic segmentation**. The dataset can be loaded into deep learning frameworks like **PyTorch** or **TensorFlow** for training models such as UNet, DeepLabV3, or UNetFormer.

### Example Code

Here’s a basic example to load the images using Python:

```python
import os
from PIL import Image

dataset_path = "path/to/DeepEarthMY_Dataset"

# Load an image from the dataset
image_path = os.path.join(dataset_path, "Rural", "image_001.png")
image = Image.open(image_path)
image.show()
