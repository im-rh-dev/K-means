# K-means Clustering and Image Quantization

## Introduction
This repository contains a Python implementation of the K-means clustering algorithm, both from scratch and using scikit-learn, with an application to image color quantization. The project is implemented in the Jupyter Notebook and demonstrates clustering data points and reducing the color palette of an image using K-means. The code is designed for educational purposes, showcasing the algorithm's mechanics and its use in image processing.

The custom K-means implementation includes functions for assigning labels, computing centroids, and tracking convergence, while the image quantization example reduces the color palette of an image (`china.jpg`) to a specified number of colors (K=8). Visualizations compare the original and quantized images.

## Features
- **Custom K-means Implementation**:
  - Computes cluster assignments based on Euclidean distance.
  - Updates centroids by calculating the mean of points in each cluster.
  - Tracks inertia (sum of squared distances to centroids) for convergence monitoring.
  - Supports configurable parameters: number of clusters (`n_clusters`), maximum iterations (`max_iter`), tolerance (`tol`), and random seed (`random_state`).
- **Image Quantization**:
  - Applies K-means to cluster pixel colors in an RGB image.
  - Reduces the image's color palette to `K=8` colors using scikit-learn's `KMeans`.
  - Visualizes the original and quantized images side-by-side using Matplotlib.
- **Visualization**:
  - Displays clustering results and image quantization outputs.
  - Plots the original image alongside the quantized version for visual comparison.
- **Validation**:
  - Compares empirical results (e.g., inertia) with theoretical expectations.
  - Demonstrates convergence of the K-means algorithm through inertia history.

## Datasets
- **Image Data**: The notebook uses an image file (`china.jpg`) for color quantization. This file is not included in the repository due to its proprietary nature. Users must provide their own image file or adapt the code to use a different image.
- **Synthetic Data**: The code includes imports for `make_blobs` from scikit-learn, which can be used to generate synthetic data for testing the K-means algorithm (though not used in the provided notebook).

## Installation
To run the code, install the required Python dependencies. The project uses standard Python libraries for numerical computation, clustering, and visualization.

### Prerequisites
- Python 3.8+
- Required libraries:
  ```bash
  pip install numpy matplotlib scikit-learn
