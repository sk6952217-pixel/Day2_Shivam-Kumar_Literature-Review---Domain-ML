## Dataset Exploration and Preprocessing

## 1. Objective

The main objective of Day 2 was to explore the underwater image dataset, understand the different image types, observe the image quality, and test a basic preprocessing step.

## 2. Dataset Exploration

The dataset was explored using Python in Google Colab.

The image categories were counted as follows:

- Input images: **1078**
- Target images: **1078**
- Generated images: **1078**
- Total categorized images: **3234**

The initial dataset inspection showed **3235 images**, resulting in a difference of one image.

## 3. Image Dimensions

The dimensions of the images were checked for each folder.

The inspected images were found to have a dimension of:

**256 × 256 pixels**

## 4. Image Visualization

Input, target, and generated images were displayed and compared.

The following observations were made:

- Target images appeared clearer than input images.
- No major color difference was observed.
- Generated images appeared closer to the target images.
- No noticeable blur or noise was observed.
- Important image details were preserved.

## 5. Preprocessing

A basic preprocessing test was performed on an input image.

The following steps were applied:

1. Image was converted to RGB format.
2. Image was resized to **256 × 256 pixels**.
3. Image was converted into a NumPy array.
4. Pixel values were normalized from **0–255 to 0–1**.

The preprocessing produced a pixel range of:

**0.0 to 0.9765**

Since the original image was already 256 × 256, its size remained unchanged after resizing.

## 6. Challenges

The main challenges observed during the exploration were:

- Understanding the organization of images into different folders.
- Identifying input, target, and generated images using their filenames.
- The total image count did not match the sorted count.

## 7. Results

The dataset was successfully explored and a preprocessing operation was tested.

The image dimensions, image categories, and visual characteristics were identified. The preprocessing test successfully converted the image to RGB, resized it, and normalized its pixel values.

## 8. Learning Outcomes

From this activity, I learned:

- How to explore an image dataset using Python.
- How to count and categorize images.
- How to check image dimensions.
- How to visualize and compare images.
- How image resizing works.
- How pixel normalization works.
- How to record observations and identify basic dataset issues.

## Conclusion

Day 2 successfully covered basic dataset exploration, image visualization, and preprocessing. The results provide a foundation for further data preprocessing and model implementation.
