# Image Compression Using Low-Rank Approximation

## Overview

This project implements image compression techniques using Singular Value Decomposition (SVD) to approximate images by retaining only the most significant singular values. The goal is to compress images by reducing their rank and minimizing the error, either using the 2-norm error or the Frobenius norm error.

### Features:
- **Low-Rank Approximation:** Decompose the image into a low-rank approximation using SVD.
- **Compression Methods:**
  - Compression based on a **2-norm error** tolerance.
  - Compression based on a **Frobenius norm error** tolerance.
- **Rank Calculation:** Automatically calculate the rank required to achieve the desired compression error.
- **Image Visualization:** Display the original and compressed images side by side for visual comparison.
- **Error Tolerance Testing:** Evaluate the compression for various tolerance values.

## Dependencies

- `numpy`: For numerical computations.
- `matplotlib`: For plotting and displaying images.
- `scipy`: (Optional) For advanced matrix operations if needed.

To install the required dependencies, you can use the following:

```bash
pip install numpy matplotlib
