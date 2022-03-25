![Bloods.ai](https://zindpublic.blob.core.windows.net/public/uploads/image_attachment/image/1026/54f4e853-d513-4328-bfcd-b9069d0c8636.png)
> [Competition](https://zindi.africa/competitions/bloodsai-blood-spectroscopy-classification-challenge) hosted by bloods.ai on [Zindi](https://zindi.africa)

# Overview
Traditionally we do blood analysis by collecting blood samples from patients and perform different tests on the samples. In this competition, you will help scientists from bloods.ai to make progress towards non-invasive blood analyses.
For this purpose, you build machine learning models that can classify the level of specific chemical compounds in samples from their spectroscopic data. In simple terms when we direct a beam of light towards a sample, the light is partially absorbed and/or reflected based on the sample's molecular structure (different chemical compounds present).

# Data Collection
Raw data is obtained as a result of the scanner shining light into the target (in this case, a fingertip). The information is presented as a function of wavelength in nanometers (nm). In order to account for all wavelength data, the results are registered as an array of values(170 intensity values per scan).

To create a reliable scan, the operation is done 60 times. Temperature and humidity are also taken into consideration. Each of the 60 scans has 170 intensities, which take into account the temperature and humidity at the time of the scan.
