# PCD Assignment 01

## Digital Image Processing — Down Sampling and Up Sampling

This repository contains the submission for PCD Assignment 01.

**Author:** Chelsea Christofera Antonioli Purnomo  
**NIM:** 25/558145/PA/23462

### Experiments
- Down Sampling: Max, Average, Median
- Up Sampling: Nearest Neighbor, Bilinear, Bicubic
- Input images: colorful garden, staircase, and batik pattern
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

### Report
`report/PCD_Assignment01_Report.pdf` contains a three-page analysis, with one page dedicated to each input image.
