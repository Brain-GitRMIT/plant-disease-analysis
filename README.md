# plant-disease-analysis
This repository contains the code and outputs for comparing a Support
Vector Machine (SVM) and a Convolutional Neural Network (CNN) using the
PlantVillage and PlantDoc plant-disease image datasets.
## Repository Files

- `plant_disease_analysis_clean.ipynb` – complete Google Colab notebook
- `final_model_results.csv` – accuracy and macro-F1 results
- `model_performance_comparison.png` – final performance comparison figure
- `selected_image_manifest.csv` – selected image URLs, labels and data splits
## Experimental Design

Eight matching tomato and bell-pepper classes were selected from both
datasets. Sixty images per class were sampled from each dataset, producing
960 images overall. Each dataset used a stratified 80:20 training and
testing split.

The SVM used flattened and normalised 64 x 64 RGB images. The CNN used
128 x 128 RGB images with image augmentation and early stopping. The
PlantVillage-trained models were also evaluated on the PlantDoc test set
to examine cross-dataset generalisation.

## Running the Notebook

The notebook is designed to run in Google Colab.

1. Open `plant_disease_analysis_clean.ipynb` in Google Colab.
2. Select **Runtime > Run all**.
3. The notebook downloads the selected images from their public sources.
4. The generated outputs are saved in the Colab `/content` directory.
An internet connection is required. The image dataset itself is not stored
in this repository.
