
## 1. Literature Review

Underwater images often suffer from problems such as low contrast, color distortion, poor visibility, and loss of image details. Different image enhancement methods can be used to improve the quality of these images.

### A. Histogram Equalization

Histogram Equalization :- is a traditional image enhancement technique that improves image contrast by redistributing pixel intensity values.

**Advantages:**
- Simple to understand and implement
- Fast processing
- Does not require training

**Limitations:**
- May over-enhance the image
- Can produce unnatural results
- Does not directly correct underwater color distortion

### B. CLAHE

Contrast Limited Adaptive Histogram Equalization (CLAHE) improves contrast in small local regions of an image. It also limits excessive contrast enhancement.

**Advantages:**
- Improves local contrast
- Preserves image details
- Usually better than standard Histogram Equalization

**Limitations:**
- Can amplify noise
- Requires suitable parameter settings

### C. Gamma Correction

Gamma Correction adjusts the brightness of an image using a mathematical power function. It can make dark underwater images brighter and improve visibility.

**Advantages:**
- Simple and fast
- Useful for correcting brightness
- Does not require training

**Limitations:**
- Mainly changes brightness
- Does not completely solve color distortion
- Incorrect gamma values can make images too bright or too dark

### D. White Balance

White Balance corrects the color cast present in underwater images by adjusting the intensity of different color channels.

**Advantages:**
- Helps correct underwater color distortion
- Simple to implement
- Fast processing
- Does not require training

**Limitations:**
- May not improve contrast significantly
- Cannot solve all types of underwater degradation

### E. Retinex-Based Enhancement

Retinex-based methods treat an image as a combination of illumination and reflectance. The method attempts to improve illumination, contrast, and details.

**Advantages:**
- Improves illumination
- Enhances image details
- Can improve contrast and color appearance

**Limitations:**
- More complex than basic enhancement methods
- May introduce artifacts
- Requires more computation

### F. CNN-Based Image-to-Image Method

CNN-based image-to-image methods use Convolutional Neural Networks to learn a mapping from a degraded underwater input image to an enhanced target image.

**Advantages:**
- Can learn complex image degradation patterns
- Can produce high-quality enhanced images
- Can preserve important image details
- Suitable for input-target image datasets

**Limitations:**
- Requires training data
- Requires more computational resources
- Training takes more time than classical methods


# 2. Comparison Table

| Method | Type | Main Purpose | Contrast Improvement | Color Correction | Brightness Correction | Detail Preservation | Computational Cost | Training Required |
|---|---|---|---|---|---|---|---|---|
| Histogram Equalization | Classical | Improve global contrast | High | Low | Moderate | Moderate | Low | No |
| CLAHE | Classical | Improve local contrast | High | Low-Moderate | Moderate | Good | Low-Medium | No |
| Gamma Correction | Classical | Adjust brightness | Moderate | Low | High | Moderate | Low | No |
| White Balance | Classical | Correct color cast | Moderate | High | Moderate | Good | Low | No |
| Retinex-Based Enhancement | Classical / Model-Based | Improve illumination and details | High | Good | High | Good | Medium | No |
| CNN-Based Image-to-Image | Deep Learning | Learn enhancement from input to target | High | High | High | High | High | Yes |


# 3. Candidate-Method List

The following six methods were selected as candidate methods for underwater image enhancement:

1. **Histogram Equalization**

     Used as a simple global contrast enhancement baseline.

2. **CLAHE**

     Used to improve local contrast and preserve image details.

3. **Gamma Correction**

     Used to improve brightness and visibility.

4. **White Balance**

     Used to correct underwater color distortion.

5. **Retinex-Based Enhancement**

     Used to improve illumination, contrast, and details.

6. **CNN-Based Image-to-Image Method**

     Used as a deep learning approach to learn enhancement from input images and target images.

   

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

## 5. Basic Preprocessing

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
- The total images count did not match the sorted count.

## 7. Results

The dataset was successfully explored and a basic preprocessing operation was tested.

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
