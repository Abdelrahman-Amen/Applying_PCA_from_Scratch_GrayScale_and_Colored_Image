# Principal Component Analysis (PCA) 📈
# What is PCA?

![Principal20Analysis20principal](https://github.com/user-attachments/assets/60129bea-86ed-4086-a5d9-e85e434ca411)


## PCA is a statistical technique used for dimensionality reduction. It transforms high-dimensional data into a smaller-dimensional subspace while retaining as much variability (information) as possible. This is achieved by finding new axes (principal components) that capture the most variance in the data.

# PCA is widely used in:

### • Image compression: Reducing image size while maintaining quality.

### • Visualization: Representing high-dimensional data in 2D or 3D.

### • Feature extraction: Selecting the most informative features for machine learning models.


# Key Steps in PCA (From Scratch)


# Data Representation:

### • Represent the data as a matrix. For images, this means converting pixel values into numerical matrices. For datasets, rows represent samples, and columns represent features.

# Mean Centering:

### • Calculate the mean of each column (feature or pixel) and subtract it from the dataset. This centers the data around the origin, simplifying subsequent calculations.

# Covariance Matrix:

### • Compute the covariance matrix of the mean-centered data. This matrix represents the variance and relationships between features.

# Eigenvalues and Eigenvectors:

### • Calculate the eigenvalues and eigenvectors of the covariance matrix.

### • Eigenvalues: Indicate the amount of variance captured by each principal component.

### • Eigenvectors: Represent the directions of the principal components.

# Sorting:

### • Sort eigenvectors based on their eigenvalues in descending order. The largest eigenvalues correspond to the directions with the most variance.

# Dimensionality Reduction:


### • Select the top k eigenvectors (based on eigenvalues) to form a reduced subspace.

### • Project the data onto this subspace to reduce its dimensionality.

# Reconstruction (Optional):


### • Multiply the reduced data by the eigenvectors and add the mean to approximate the original data.



# Applying PCA to Different Scenarios

# Grayscale Images:
### • Grayscale images are single-channel images where pixel intensity values range from 0 to 255.

## • Steps:

### 1. Convert the image into a 2D matrix.

### 2. Perform mean centering and covariance matrix computation.

### 3. Apply PCA to reduce dimensions. 

### 4. Reconstruct the image using the reduced components.

### •  Goal: Compress the image by reducing the number of principal components while maintaining visual quality.


# Colored Images:
### • Colored images have three channels: Red (R), Green (G), and Blue (B).
## Steps:

### 1. Split the image into R, G, and B channels.

### 2. Perform PCA separately for each channel following the grayscale image steps.

### 3. Reconstruct the image by combining the processed R, G, and B channels.

### • Goal: Achieve compression or dimensionality reduction while retaining color fidelity.


# Datasets (e.g., Olivetti Faces):
### • The Olivetti Faces dataset is a collection of 400 grayscale face images. Each image is 64x64 pixels, representing a flat vector (4096 features per image).

## • Steps:

### 1. Directly apply PCA to the dataset, where each row represents an image and columns represent pixel values.
 
### 2. Reduce the dimensionality of the dataset while preserving the most important features.
### • Goal: Capture the most significant facial features for tasks like recognition or reconstruction.



# Key Differences Between Scenarios:
![a](https://github.com/user-attachments/assets/af70f20f-bd45-46bb-99ea-be3ad1fc3448)


