# Khmer Character Recognition 


This repository contains a Python script that generates images with Khmer script labels, such as digits and characters, using random khmer fonts and rotations. These images are saved as PNG files for use in training Khmer character recognition models. Additionally, the images are processed and stored in CSV format.

## Features

- **Random Label Generation**: The script generates images of random Khmer digits and characters from a predefined list.
- **Random Font Selection**: The script selects a random font from a ZIP archive containing `.ttf` font files.
- **Random Rotation**: The text in each image is randomly rotated by an angle between -10 and 10 degrees to create variety.
- **Unique Image Filenames**: Each generated image is saved with a unique filename based on the label, font, and rotation angle to avoid overwriting.
- **Output Directory**: All generated images are stored in the `labels/` directory.
- **CSV Conversion**: The images are flattened and saved as a CSV file, where each row contains the label followed by 784 pixel values (for 28x28 images).



**Here are some generated images of Khmer characters:**

![Khmer Character 1](ញ_0_-1.png)

![Khmer Character 2](ក_18_2.png)
     
![Khmer Character 3](គ_25_-2.png)

![Khmer Character 3](ឈ_13_5.png)


## Requirements

To use this Khmer Character Recognition Image Generator, you need the following Python packages:

- **[Python 3.x](https://www.python.org/)** ![Python](https://img.shields.io/badge/Python-3.x-blue)
- **[Pillow](https://pillow.readthedocs.io/en/stable/)** – for image creation and manipulation ![Pillow](https://img.shields.io/badge/Pillow-8.2.0-blue)
- **[numpy](https://numpy.org/doc/stable/)** – for array operations ![numpy](https://img.shields.io/badge/numpy-1.21.0-blue)
- **[pandas](https://pandas.pydata.org/pandas-docs/stable/)** – for CSV manipulation ![pandas](https://img.shields.io/badge/pandas-1.3.0-blue)
- **[scikit-learn](https://scikit-learn.org/stable/)** – for machine learning (model training, evaluation) ![scikit-learn](https://img.shields.io/badge/scikit--learn-0.24.0-blue)
- **[imbalanced-learn](https://imbalanced-learn.org/stable/)** – for balancing the dataset using SMOTE ![imbalanced-learn](https://img.shields.io/badge/imbalanced--learn-0.8.0-blue)
- **Built-in libraries**: os, csv, random, io, zipfile

You can install the necessary libraries using the following command:

```bash
pip install pillow numpy pandas scikit-learn imbalanced-learn
