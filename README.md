# BME3053C FinalProject
## Breast Cancer Detection on Ultrasounds

### Overview
This MATLAB project aims to detect breast cancer on ultrasound images using image processing techniques. We utilized a dataset of 780 ultrasound images containing malignant and benign tumors, as well as normal scans with no tumors. We limited our sample size to 30 for this project. Our approach involves converting the images to grayscale, detecting edges, applying morphological operations (imclose and imfill), clearing the border to create a tumor boundary, and calculating circularity to identify round/oval shaped components. The largest circular-shaped region, meeting a minimum area criteria, is identified as the tumor. A mask is then created and overlaid on top of the original scan to highlight the tumor, if present.

### Methodology
Preprocessing: Convert images to grayscale.

Edge Detection: Detect edges using appropriate algorithms.

Morphological Operations: Apply imclose and imfill functions to enhance tumor boundaries.

Circularity Calculation: Calculate circularity for each component to identify round/oval shapes.

Tumor Identification: Identify the largest circular-shaped region meeting a minimum area criterion as the tumor.

Mask Overlay: Create a mask and overlay it on the original scan to highlight the tumor, if present.

### Limitations
Small Dataset: Our approach was tested on a limited dataset of 30 images. Results may vary with larger datasets.

Limited Tumor Contrast: The approach works best when tumors exhibit high contrast with the background.

False Positives: Healthy tissue is occasionally mistaken for benign tumors, occurring approximately 30% of the time. This may be attributed to the nature of ultrasounds, which can produce false positives frequently.

### Future Work
Improved Tumor Classification: Explore methods to distinguish between malignant and benign tumors more accurately.

Larger Dataset: Expand the dataset to improve the robustness and generalization of the model.

Enhanced Performance: Investigate techniques to improve performance on ultrasounds with low tumor contrast.

Clinical Validation: Collaborate with medical professionals to validate the effectiveness of the approach on clinical data.

### Contributors
Ayushi Elhence - ayushi.elhence@ufl.edu 
Moie Brenner - moiebrenner@ufl.edu
Grace Koch - grace.koch@ufl.edu
