# Color Quantization using KMeans Clustering

This project applies KMeans clustering for color quantization or palette generation on digital images. The goal is to reduce the number of colors in an image while preserving its visual quality as much as possible.

## Problem

Digital images often contain thousands of colors. For applications like compression, thumbnails, etc fewer colors are preferred while maintaining image appearance. 

## Method

The steps are:

1. Read RGB values of pixels and represent as data points in 3D space
2. Define number of clusters k using Elbow method
3. Perform KMeans clustering to group pixels  
4. Assign cluster centroid color to each pixel
5. Render new image and compare with original

## Data

A sample palm tree image containing 262144 pixels in JPG format.

## Usage

- Image compression 
- Vector quantization
- Generating color swatches
- Digital art color palette design

## Demo

The notebook demonstrates color quantization on the sample image from 262144 to 64 colors. It is able to largely preserve visual quality while reducing colors by 96.5%.

## Requirements

- Python
- Scikit-learn 
- NumPy, Matplotlib
- PIL (for loading/saving images)
