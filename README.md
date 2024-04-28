# Image-Matching-using-SIFT-Algorithm

---

# Image Matching and Object Localization

This repository contains Python scripts for performing image matching using different feature detectors and descriptors such as SIFT, BRIEF, and ORB, as well as object localization using a pre-trained object detection model. These scripts are useful for tasks like image registration, finding correspondences between images, and detecting objects in images.

## Prerequisites

- Python 3.x
- OpenCV (`opencv-python`)
- Matplotlib (`matplotlib`)
- Torchvision (`torchvision`)
- Torch (`torch`)

We can install the required packages using pip:

```
pip install opencv-python matplotlib torch torchvision
```

## Usage

### Image Matching with SIFT Detector

The script `sift_image_matching.py` performs image matching using the Scale-Invariant Feature Transform (SIFT) detector. It calculates matches between keypoints detected in two input images and displays the matches along with the images.

Example usage:
```python
image1_path = "/path/to/image1.jpg"
image2_path = "/path/to/image2.jpg"
calculate_matches(image1_path, image2_path, score_threshold=20.0)
```

### Image Matching with BRIEF Descriptor

The script `brief_image_matching.py` performs image matching using the Binary Robust Independent Elementary Features (BRIEF) descriptor. It detects keypoints using the FAST detector and computes BRIEF descriptors for matching.

Example usage:
```python
image1_path = "/path/to/image1.jpg"
image2_path = "/path/to/image2.jpg"
calculate_matches(image1_path, image2_path, score_threshold=20.0)
```

### Image Matching with ORB Detector

The script `orb_image_matching.py` performs image matching using the Oriented FAST and Rotated BRIEF (ORB) detector. It detects keypoints and computes ORB descriptors for matching.

Example usage:
```python
image1_path = "/path/to/image1.jpg"
image2_path = "/path/to/image2.jpg"
calculate_matches(image1_path, image2_path, score_threshold=20.0)
```

### Object Localization with Faster R-CNN

The script `object_localization.py` performs object localization using a pre-trained Faster R-CNN model. It detects objects in two input images and draws bounding boxes around the detected objects.

Example usage:
```python
image1_path = "/path/to/image1.jpg"
image2_path = "/path/to/image2.jpg"
sift_feature_matching(image1_path, image2_path)
```
