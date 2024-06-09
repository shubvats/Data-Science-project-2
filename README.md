# K-Means Image Segmentation

## Overview
This MATLAB script implements the K-Means clustering algorithm for image segmentation. It takes an array of images as input and performs K-Means clustering for various values of K, generating segmented images and heatmaps.

## Motivation
Image segmentation is a crucial task in computer vision and image processing. K-Means clustering provides a simple yet effective method for partitioning images into distinct regions, enabling various applications such as object recognition, image compression, and feature extraction.

## Usage

### Requirements
- MATLAB R2016a or later.

### Instructions
1. Clone or download this repository to your local machine.
2. Open MATLAB and navigate to the directory containing the script.
3. Define your input images in `imageArray` variable in `main.m`.
4. Set the desired values of K (number of clusters) in `kValues`.
5. Specify the tolerance value for convergence in the `tolerance` variable.
6. Run the `main.m` script.

```matlab
% Example usage
imagePaths = {'image1.jpg', 'image2.jpg', ...}; % Array of image paths
kValues = [2, 3, 4]; % Array of K values
tolerance = 0.001; % Tolerance value for convergence
main(imagePaths, kValues, tolerance);
```

## Functionality

### `main(imageArray, kValues, tolerance)`
- This function orchestrates the entire process:
  - Reads each image from `imageArray`.
  - Performs K-Means clustering for different values of K specified in `kValues`.
  - Displays the original image and the corresponding heatmap after clustering.

### `displayResults(inputImage, clusteredImage, numClusters, imageName)
- This function visualizes the results by displaying the original image and the heatmap generated after clustering.

## Results
The script generates segmented images and heatmaps for each input image, providing insights into the effectiveness of K-Means clustering for image segmentation.

## Contributions
Contributions and feedback are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## Acknowledgments
- The K-Means clustering algorithm is implemented using MATLAB's built-in `kmeans` function.
- Initial inspiration and guidance from [MATLAB documentation](https://www.mathworks.com/help/stats/kmeans.html).

--- 

Feel free to customize and enhance this README to better suit your project!
