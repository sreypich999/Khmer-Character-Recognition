# Khmer Character Recognition Image Generator

This repository contains a Python script that generates images with Khmer script labels, such as digits and characters, using random fonts and rotations. These images are saved as PNG files for use in training Khmer character recognition models.

## Features

- **Random Label Generation**: The script generates images of random Khmer digits and characters from a predefined list.
- **Random Font Selection**: The script selects a random font from a ZIP archive containing `.ttf` font files.
- **Random Rotation**: The text in each image is randomly rotated by an angle between -10 and 10 degrees to create variety.
- **Unique Image Filenames**: Each generated image is saved with a unique filename based on the label, font, and rotation angle to avoid overwriting.
- **Output Directory**: All generated images are stored in the `labels/` directory.

## Requirements

- Python 3.x
- `Pillow` (for image creation and manipulation)
- `os`, `zipfile`, `random`, `io` (standard Python libraries)

To install the necessary libraries, you can run the following:

```bash
pip install pillow
