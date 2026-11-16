# Image Processing Lab

**A hands-on exploration of digital image processing, mathematical foundations, and computer vision using Python.**

## Overview

Image Processing Lab is a collection of educational Jupyter notebooks designed to explore the mathematical and computational foundations of digital image processing.

The project combines theoretical explanations, implementations using NumPy, visual experiments, and comparisons with established computer vision libraries such as OpenCV and scikit-image.

The goal is to develop a deeper understanding of how digital images are represented, transformed, enhanced, and analyzed, while building a foundation for more advanced topics in computer vision, signal processing, and deep learning.

## Learning Objectives

- Understand the numerical representation of digital images.
- Explore RGB color channels, grayscale conversion, and intensity transformations.
- Analyze image histograms and contrast enhancement techniques.
- Implement fundamental image processing algorithms using NumPy.
- Understand spatial filtering, convolution, and Gaussian smoothing.
- Compare custom implementations with established library functions.
- Investigate the mathematical connections between image processing, signal processing, and computer vision.

## Technologies

| Technology | Purpose |
|---|---|
| Python | Programming and experimentation |
| NumPy | Numerical computation and image arrays |
| Matplotlib | Image visualization and plotting |
| OpenCV | Computer vision and image processing algorithms |
| scikit-image | Image processing algorithms and sample datasets |
| SciPy | Scientific computing and signal processing |
| Pillow | Image loading and manipulation |
| Jupyter | Interactive experiments and documentation |
| pytest | Testing and validation |

## Experiments

The laboratory is organized into seven introductory notebooks.

| Notebook | Topic | Key Concepts |
|---|---|---|
| 01 | Digital Images | Pixels, arrays, resolution, data types, quantization |
| 02 | RGB & Grayscale | Color channels, luma, luminance, grayscale conversion |
| 03 | Histograms & Contrast | Intensity distributions, contrast stretching, quantization |
| 04 | Histogram Equalization | Probability distributions, CDF, lookup tables |
| 05 | CLAHE | Adaptive contrast enhancement, local histograms, clip limits |
| 06 | Convolution & Filtering | Spatial kernels, padding, correlation, convolution |
| 07 | Gaussian Blur | Gaussian distributions, spatial smoothing, sigma, frequency response |

### 01 — Digital Image Representation

Explores digital images as multidimensional numerical arrays, including pixel values, channel organization, memory representation, and quantization.

### 02 — RGB and Grayscale

Examines RGB color channels and mathematical approaches to grayscale conversion, including the distinction between luma and linear-light luminance.

### 03 — Image Histograms and Contrast

Introduces intensity histograms, contrast stretching, low-contrast image simulation, and the effects of quantization and intensity outliers.

### 04 — Histogram Equalization

Implements histogram equalization using probability distributions, cumulative distribution functions, and lookup tables, with numerical comparisons against OpenCV.

### 05 — CLAHE

Investigates Contrast Limited Adaptive Histogram Equalization, local intensity transformations, and the effects of clip limits and tile grid configurations.

### 06 — Convolution and Spatial Filtering

Explores convolution kernels, neighborhood operations, mean filtering, boundary handling, and the distinction between mathematical convolution and cross-correlation.

### 07 — Gaussian Blur

Studies Gaussian kernels, their mathematical properties, the influence of sigma, separable filtering, and the relationship between Gaussian smoothing and spatial frequencies.

## Experimental Approach

Each notebook combines several components:

1. **Mathematical Foundations:** Theoretical concepts and relevant equations.
2. **Algorithm Implementation:** Practical implementations, including NumPy-based methods.
3. **Visual Experiments:** Image comparisons, plots, and parameter exploration.
4. **Library Validation:** Comparisons against established implementations where applicable.
5. **Interpretation:** Discussion of observed results, limitations, and practical implications.
6. **Review Questions:** Opportunities to reinforce conceptual understanding.

The emphasis is on understanding not only how an algorithm works, but also why it works and when it may be useful.

## Installation

### Prerequisites

- Python 3.10 or a compatible version
- Git
- Jupyter Notebook or Visual Studio Code with the Python and Jupyter extensions

### 1. Clone the repository

```bash
git clone https://github.com/<YOUR-USERNAME>/image-processing-lab.git
cd image-processing-lab
```

Replace `<YOUR-USERNAME>` with your GitHub username.

### 2. Create a virtual environment

**macOS / Linux**

```bash
python3 -m venv .venv
source .venv/bin/activate
```

**Windows (PowerShell)**

```powershell
py -3.10 -m venv .venv
.\.venv\Scripts\Activate.ps1
```

If Python 3.10 is unavailable, use another compatible installed Python version.

### 3. Install dependencies

```bash
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

### 4. Launch the notebooks

Open the project in Visual Studio Code, select the Python interpreter from `.venv`, and open any notebook.

Alternatively, register the environment as a Jupyter kernel:

```bash
python -m ipykernel install --user --name image-processing-lab --display-name "Image Processing Lab"
```

Select the corresponding kernel and execute the notebook cells in order.

## Sample Images

The experiments use built-in sample images provided by `scikit-image`, including:

- `skimage.data.astronaut()` — RGB image experiments.
- `skimage.data.camera()` — Grayscale image processing experiments.

These examples allow experiments to run without downloading additional image datasets.

Image credits and licensing information are available in the [scikit-image documentation](https://scikit-image.org/docs/stable/api/skimage.data.html).

## Reproducibility

The notebooks are designed to execute independently using standard Python scientific computing libraries.

Where applicable, custom implementations are compared against OpenCV or scikit-image to examine numerical consistency and algorithmic behavior.

Results may vary slightly depending on library versions, floating-point precision, and execution environment.

## Future Topics

Planned areas of exploration include:

- Image Gradients and Sobel Operators
- Canny Edge Detection
- Laplacian and Sharpening Filters
- Fourier Transform and Frequency-Domain Processing
- Image Segmentation
