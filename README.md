![Bloods.ai](https://zindpublic.blob.core.windows.net/public/uploads/image_attachment/image/1026/54f4e853-d513-4328-bfcd-b9069d0c8636.png)
> My solution to [Blood Spectroscopy Challenge](https://zindi.africa/competitions/bloodsai-blood-spectroscopy-classification-challenge) hosted by bloods.ai on [Zindi](https://zindi.africa) to perform blood analysis non invasively by using spectral data gotten from NIR(Near Infra-Red).

# Overview
Traditionally we do blood analysis by collecting blood samples from patients and perform different tests on the samples. In this competition, you will help scientists from bloods.ai to make progress towards non-invasive blood analyses.
For this purpose, you build machine learning models that can classify the level of specific chemical compounds in samples from their spectroscopic data. In simple terms when we direct a beam of light towards a sample, the light is partially absorbed and/or reflected based on the sample's molecular structure (different chemical compounds present).

# Data Collection
Raw data is obtained as a result of the scanner shining light into the target (in this case, a fingertip). The information is presented as a function of wavelength in nanometers (nm). In order to account for all wavelength data, the results are registered as an array of values(170 intensity values per scan).

To create a reliable scan, the operation is done 60 times. Temperature and humidity are also taken into consideration. Each of the 60 scans has 170 intensities, which take into account the temperature and humidity at the time of the scan.

## Bilogical Window
On the electromagnetic spectrum, NIR spectra cover the wavelength range of 750-2500 nm. This is known as the biological window, and it is within this range that we will be working on this problem. We can collect signatures of chemical substances present in blood that flows close to the skin's surface blood vessels in this way. The penetration depth in millimeters of each wavelength over the near infrared band is depicted in the diagram below.

<img src="https://github.com/blackhat-coder/Blood-Spectroscopy/blob/master/imgs/Biologicalwindow.JPG" width="500" height="250">
 
## Spectral Signature of Compounds
<img src="https://github.com/blackhat-coder/Blood-Spectroscopy/blob/master/imgs/cholesterol.JPG" width="200" height="200"><img src="https://github.com/blackhat-coder/Blood-Spectroscopy/blob/master/imgs/Glucose.JPG" width="200" height="200"><img src="https://github.com/blackhat-coder/Blood-Spectroscopy/blob/master/imgs/hemoglobin.JPG" width="200" height="200">
 
Cholesterol Signature Graph, Glucose Signature Graph, Hemoglobin Signature Graph (From Left to Right)

# Setup
- Download [Data Files](https://zindi.africa/competitions/bloodsai-blood-spectroscopy-classification-challenge/data)
- Unzip `Additional_hdl_rows_483.zip` `Additional_ldl_rows_410.zip` `Additional_hgb_rows_965_LOW_STD.zip` `Additional_ldl_rows_135_LOW_STD.zip` `Additional_hgb_rows_2457.zip` `Additional_hdl_rows_162_LOW_STD.zip`
```bash
 >> git clone https://github.com/blackhat-coder/Blood-Spectroscopy/
 ```
- Navigate to Working Directory `/Blood-Spectroscopy/`, Run:
```bash
 >> mkdir Additional
 ```
```bash
 >> pip install -r requirements.txt
```

# Usage(Jupyter Notebook)
Open `EDA.ipynb` to access source codes. You can also make edits to suite your hacking style ☺

You can access `Findings.txt` to explore some of my ideas.

# Acknowledgements
Some of the things I found useful while tackling this challenge
- [SpectraAI](https://github.com/conor-horgan/spectrai) : Even though I had a hard time setting up and probably didn't use it. SpectraAI provides a deep learning framework to facilitate the training of neural networks on spectral data.
## Papers
- Conor C. Horgan and Mads S. Bergholt, "spectrai: a deep learning framework for spectral data.", [arXiv preprint arXiv:2108.07595 (2021)](https://arxiv.org/abs/2108.07595).

# Hardware Requirements
- A computer with CPU :) 
- A cup of cofee ☕

# Licence
[![License: MIT](https://img.shields.io/badge/License-MIT-red.svg)](https://github.com/blackhat-coder/Blood-Spectroscopy/blob/master/LICENCE)

