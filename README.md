# K-Means Clustering and PCA - Exercise 7

Machine Learning course exercises for K-Means clustering and Principal Component Analysis.

## Quick Start

### Run K-Means Exercise (ex7)

```bash
octave --eval "pkg load statistics; ex7"
```

### Run PCA Exercise (ex7_pca)

```bash
octave --eval "pkg load statistics; ex7_pca"
```

### Interactive Mode

Start Octave and run exercises interactively:

```bash
octave
```

Then in Octave:

```matlab
pkg load statistics
ex7          % Run K-Means exercise
ex7_pca      % Run PCA exercise
```

## Setup (First Time Only)

### 1. Install Octave

```bash
brew install octave
```

### 2. Install Statistics Package

```bash
octave --eval "pkg install -forge statistics"
```

## Exercises

- **ex7.m** - K-Means clustering algorithm

  - Finding closest centroids
  - Computing centroid means
  - K-Means on example dataset
  - Image compression using K-Means

- **ex7_pca.m** - Principal Component Analysis
  - Dimensionality reduction
  - Visualization of reduced dimensions
  - Face image reconstruction

## Files

### Main Exercise Scripts

- `ex7.m` - K-Means clustering exercise
- `ex7_pca.m` - PCA exercise

### Data Files

- `ex7data1.mat` - Example dataset for K-Means
- `ex7data2.mat` - Example dataset for K-Means
- `ex7faces.mat` - Face images for PCA
- `bird_small.mat` - Bird image for K-Means compression

### Helper Functions

- `findClosestCentroids.m` - Find closest centroids
- `computeCentroids.m` - Compute centroid means
- `kMeansInitCentroids.m` - Initialize K-Means centroids
- `runkMeans.m` - Run K-Means algorithm
- `pca.m` - PCA implementation
- `projectData.m` - Project data onto principal components
- `recoverData.m` - Recover data from principal components
- `featureNormalize.m` - Normalize features
- `displayData.m` - Display data as images
- `plotDataPoints.m` - Plot data points
- `plotProgresskMeans.m` - Visualize K-Means progress
- `drawLine.m` - Draw a line

## Notes

- The statistics package is required for the `pdist` function
- Plots will open in separate windows during execution
- Press Enter to continue through the exercises
- You can run individual functions in Octave for testing

## Troubleshooting

### Error: 'pdist' undefined

Make sure to load the statistics package:

```bash
octave --eval "pkg load statistics; ex7"
```

### Graphics Issues

If plots don't display correctly, try:

```matlab
graphics_toolkit('qt')  % or 'gnuplot' or 'fltk'
```

## Resources

- Octave Documentation: https://octave.org/doc/
- Statistics Package: https://gnu-octave.github.io/packages/statistics/
