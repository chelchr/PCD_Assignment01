# PCD Assignment 01

## Digital Image Processing — Down Sampling and Up Sampling

This repository contains the submission for PCD Assignment 01.

**Author:** Chelsea Christofera Antonioli Purnomo  
**NIM:** 25/558145/PA/23462

### Experiments
- Down Sampling: Max, Average, Median
- Up Sampling: Nearest Neighbor, Bilinear, Bicubic
- Input images:
  1. Colorful Image — contains multiple colors, objects, and textures.
  2. Staircase Image — contains strong edges, geometric structures, and repetitive lines.
  3. Batik Image — contains repetitive patterns, fine textures, and color transitions.
- Evaluation: visual comparison, MSE, and PSNR

### Repository Structure
```text
PCD_Assignment01/
├── PCD_Assignment01.ipynb
├── dataset/
│   ├── image1_colorful.jpg
│   ├── image2_staircase.jpeg
│   └── image3_batik.jpg
├── results/
│   ├── metrics.csv
│   ├── *_downsampled.png
│   └── *_reconstructions.png
├── report/
│   └── PCD_Assignment01_Report.pdf
└── README.md
```

### How to Run
1. Open `PCD_Assignment01.ipynb` in Google Colab.
2. Run the cells from top to bottom.
3. When prompted, upload the three images from the `dataset` folder.
4. Review the visual comparisons and the MSE/PSNR table.
5. The generated files will appear in the `results/` folder.

### Method
Each image is downsampled by a factor of 2 using 2×2 pixel blocks. The result is then upsampled back to the original dimensions using Nearest Neighbor, Bilinear, or Bicubic interpolation.

Down sampling reduces spatial resolution by aggregating pixels within local 2×2 neighborhoods.
1. Max: selects the maximum pixel value.
2. Average: calculates the arithmetic mean.
3. Median: selects the median value.

Up sampling increases spatial resolution by estimating new pixel values.
1. Nearest Neighbor: uses the nearest existing pixel.
2. Bilinear: estimates values using neighboring pixels and linear interpolation.
3. Bicubic: uses cubic interpolation over a larger neighborhood.

### Evaluation
The reconstructed images are evaluated using:
1. Mean Squared Error (MSE)
2. Peak Signal-to-Noise Ratio (PSNR)
3. Visual comparison
A lower MSE and higher PSNR indicate greater numerical similarity to the original image.

### Tools
Python - NumPy - Panda - Matplotlib - Bantal - IPython - Google Colab 

### Report
`report/PCD_Assignment01_Report.pdf` contains a three-page analysis, with one page dedicated to each input image.
