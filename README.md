<div align="center">
<img src="https://github.com/cemac/LIFD_ENV_ML_NOTEBOOKS/blob/main/images/LIFDlogo.png"></a>
<a href="https://www.cemac.leeds.ac.uk/">
  <img src="https://github.com/cemac/cemac_generic/blob/master/Images/cemac.png"></a>
  <br>
</div>

# Leeds Institute for Fluid Dynamics Machine Learning For Earth Sciences

# Image Segmentation

[![GitHub release](https://img.shields.io/github/release/cemac/LIFD_ImageSegmentation.svg)](https://github.com/cemac/LIFD_ImageSegmentation/releases) [![GitHub top language](https://img.shields.io/github/languages/top/cemac/LIFD_ImageSegmentation.svg)](https://github.com/cemac/LIFD_ImageSegmentation) [![GitHub issues](https://img.shields.io/github/issues/cemac/LIFD_ImageSegmentation.svg)](https://github.com/cemac/LIFD_ImageSegmentation/issues) [![GitHub last commit](https://img.shields.io/github/last-commit/cemac/LIFD_ImageSegmentation.svg)](https://github.com/cemac/LIFD_ImageSegmentation/commits/master) [![GitHub All Releases](https://img.shields.io/github/downloads/cemac/LIFD_ImageSegmentation/total.svg)](https://github.com/cemac/LIFD_ImageSegmentation/releases) ![GitHub](https://img.shields.io/github/license/cemac/LIFD_ImageSegmentation.svg)[![DOI](https://zenodo.org/badge/366734586.svg)](https://zenodo.org/badge/latestdoi/366734586)

[![LIFD_ENV_ML_NOTEBOOKS](https://github.com/cemac/LIFD_ImageSegmentation/actions/workflows/python-package-conda-DR.yml/badge.svg)](https://github.com/cemac/LIFD_ImageSegmentation/actions/workflows/python-package-conda-DR.yml)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/cemac/LIFD_ImageSegmentation/HEAD?labpath=DimensionalityReduction.ipynb)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/cemac/LIFD_ImageSegmentation/blob/main/LIFD_dimensionality_reduction_colab.ipynb)

This Jupyter notebook demonstrates how artificial neural networks (ANNs) can be applied to image segmentation problems. Segmentation in this context refers to the task of assigning discrete labels to individual pixels or regions of an image. We can use segmentation models to identify and locate features of interest within an image. This notebook contains a simple application to self-driving cars, where we train a segmentation model to identify important features in dashcam footage, as well as a more complicated example, based on the work of [Coney et al. (2023)](https://doi.org/10.1002/qj.4592), identifying and characterising trapped lee waves over the UK.

## Quick look

### Quick start

**Binder and Colab buttons**

Will launch this tutorial in binder (CPU) or Google Colab (GPU).

**Running locally**

If you're already familiar with Git, Anaconda and virtual environments, the environment you need to create is found in [unet.yml](https://github.com/cemac/LIFD_ImageSegmentation/blob/main/unet.yml) and the code below will install, activate and launch the notebook. The .yml file has been tested on the latest Linux, macOS and Windows operating systems.

```bash
git clone git@github.com:cemac/LIFD_ImageSegmentation.git
cd LIFD_ImageSegmentation
conda env create -f unet.yml
conda activate unet
jupyter-notebook
```

## Installation and requirements

This notebook is designed to run on a laptop with no special hardware required. However, training of neural networks can take a long time (hours) without dedicated GPU hardware. If you have a GPU, it is recommended to do a local installation as outlined in the repository [howtorun](https://github.com/cemac/LIFD_ENV_ML_NOTEBOOKS/howtorun.md) and [jupyter_notebooks](https://github.com/cemac/LIFD_ENV_ML_NOTEBOOKS/jupyter_notebooks.md) sections. Otherwise, online compute platforms which offer GPU access (e.g. Google Colab) are strongly recommended.

## Licence Information

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">LIFD_ENV_ML_NOTEBOOKS</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="http://cemac.leeds.ac.uk/" property="cc:attributionName" rel="cc:attributionURL">CEMAC</a> are licenced under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.

## Acknowledgements

Thanks to Jonathan Coney for making available the code on which this notebook is based. This tutorial is part of the [LIFD_ENV_ML_NOTEBOOKS](https://github.com/cemac/LIFD_ENV_ML_NOTEBOOKS) series. Please refer to the parent repository for full acknowledgements.
