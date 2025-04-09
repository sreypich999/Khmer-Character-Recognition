#  Khmer Character Recognition

[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)](https://www.python.org/)
[![Pillow](https://img.shields.io/badge/Pillow-8.2.0-blue)](https://pillow.readthedocs.io/en/stable/)
[![NumPy](https://img.shields.io/badge/numpy-1.21.0-blue)](https://numpy.org/doc/stable/)
[![Pandas](https://img.shields.io/badge/pandas-1.3.0-blue)](https://pandas.pydata.org/)
[![Scikit-learn](https://img.shields.io/badge/scikit--learn-0.24.0-blue)](https://scikit-learn.org/stable/)
[![Imbalanced Learn](https://img.shields.io/badge/imbalanced--learn-0.8.0-blue)](https://imbalanced-learn.org/stable/)

A Python-based dataset generator and image processor for Khmer character recognition tasks. This tool creates PNG images of Khmer script (characters and digits), applies font and rotation augmentations, and exports the dataset into CSV format for model training.

---

## ✨ Features

- 🔡 **Random Label Generation**: Create diverse Khmer digits and characters from a predefined list.
- 🎨 **Random Font Selection**: Randomly choose fonts from a `.zip` archive of Khmer `.ttf` fonts.
- 🔄 **Rotation Augmentation**: Add random rotation (-10° to 10°) to simulate real handwriting variance.
- 🖼️ **Unique Image Naming**: Combines label, font, and rotation angle to prevent overwriting.
- 📁 **Image Output Directory**: Saves images to the `labels/` directory.
- 📊 **CSV Export**: Converts 28×28 images to flattened pixel arrays for model training (`label, pixel1, ..., pixel784`).

---

## 🖼️  Outputs

Here are some sample generated images of Khmer characters:

| Character | Image |
|-----------|-------|
| ញ        | ![Khmer Character 1](ញ_0_-1.png) |
| ក        | ![Khmer Character 2](ក_18_2.png) |
| គ        | ![Khmer Character 3](គ_25_-2.png) |
| ឈ        | ![Khmer Character 4](ឈ_13_5.png) |

---

## 🛠️ Requirements

Install all dependencies using `pip`:

```bash
pip install pillow numpy pandas scikit-learn imbalanced-learn
