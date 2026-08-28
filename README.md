
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