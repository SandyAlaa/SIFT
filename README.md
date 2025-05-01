# SIFT Feature Detection and Matching

This project demonstrates the use of the Scale-Invariant Feature Transform (SIFT) algorithm for detecting and matching keypoints between images with different transformations, such as rotation, zoom, and flipping.

## Requirements

To run the code, you need to have Python installed along with the following libraries:

- `opencv-python`
- `numpy`

You can install these dependencies using pip:

```bash
pip install opencv-python numpy
```

## Code Overview

The project includes multiple scripts for performing SIFT feature detection and matching in various image transformation scenarios:

1. **Keypoint Detection and Saving Image with Keypoints:**
   - Detects keypoints and computes descriptors from the input image.
   - Draws and saves the image with keypoints.

2. **Image Matching (Original vs Rotated):**
   - Loads two images and detects keypoints.
   - Matches keypoints between an original and a rotated version of the image using FLANN-based matching.
   - Saves the image with matched keypoints.

3. **Image Matching (Original vs Zoomed):**
   - Detects and matches keypoints between an original image and its zoomed-in version.
   - Saves the matched image.

4. **Image Matching (Original vs Flipped):**
   - Detects and matches keypoints between an original image and its flipped version.
   - Saves the matched image.

## Input Files

For all scripts, make sure to update the file paths for the input images in the code:

- `image_path = "D:\\CV codes and projects\\download.jpeg"`
- `image1_path = "D:\\CV codes and projects\\download.jpeg"`
- `image2_path = "D:\\CV codes and projects\\download2.jpeg"`

Adjust the `image_path` and `output_path` variables based on your directory structure.

## How to Run

1. Ensure you have the necessary dependencies installed (as mentioned above).
2. Place the images you want to use in the specified directories.
3. Run each script separately depending on which functionality you need:

```bash
python sift_keypoint_detection.py
python sift_image_matching_rotated.py
python sift_image_matching_zoomed.py
python sift_image_matching_flipped.py
```

## Output

Each script saves the output image with the matched keypoints to the specified `output_path`.

For example:
- `output_path = "D:\\CV codes and projects\\matched_rotated.jpeg"`

You can adjust the output paths and filenames as needed.
