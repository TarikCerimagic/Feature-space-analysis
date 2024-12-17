# Feature Space Embeddings Visualization of Cholestasis Data

This project provides a streamlined pipeline for performing dimensionality reduction and visualizing feature space embeddings. Using `UMAP`, `PCA`, and `t-SNE`, the project allows researchers to analyze and plot embeddings derived from descriptors.

---

## Table of Contents

1. [Overview](#overview)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Testing](#testing)
7. [Acknowledgements](#acknowledgements)
8. [License](#license)

---

## Overview

The project reads a CSV file containing cholestasis data, performs dimensionality reduction, and visualizes the results in a scatter plot. Labels and colors are used to differentiate cholestasis conditions, aiding in better understanding of the feature space.

---

## Features

- **Dimensionality Reduction**:
  - Supports UMAP, PCA, and t-SNE for embedding generation.
  - Easily switch between models with a single parameter.

- **Data Visualization**:
  - Scatter plots of embeddings with color-coded and marker-based differentiation.
  - Configurable plot aesthetics for publication-quality graphics.

- **Extensibility**:
  - Modular functions for dimensionality reduction and visualization.
 
## Installation

### Environment installation

YAML file can be used to install the environment for windows.

- [chemical_space_env_win.yaml](./chemical_space_env_win.yaml): Windows YAML file.

### Prerequisites

Ensure you have the following Python libraries with corresponding versions installed:
- `umap-learn` (0.5.6)
- `scikit-learn` (1.5.1)
- `matplotlib` (3.9.1)
- `pandas` (2.2.2)
- `numpy` (1.26.4)
- `ipykernel` (6.29.5)

## Usage

### Getting started

- Download the files from the repository
- Intall the required libraries manually or via YAML file
- Open [feature_space.ipynb](./feature_space.ipynb) file and select the installed environment

### Using the Jupyter Notebook

- Iport the packages
- Import one of the datasets from [data](./data) as a Pandas DataFrame
- Remove non-feature columns
- Convert the descriptor DataFrame into a NumPy array
- Run the "dimension_reduction" function
- Execute the function by setting the descriptor array and selcted type of the model (ex. "umap") as input parameters
- Add lables to x and y embeddings
- Plot the feature space

To achieve the same results, please use predifined column names for removal, hyperparameters for the UMAP model, and original datasets from the repository.

## Testing

To ensure that identical results are obtained, scatter plots are provided in [reuslts](./results) for comparison.

Jupyter Notebook can be modified to perform dimensionality reduction of other datasets. The corresponding variables should be adjusted for different data formats. Different dimensionality reduction methods can be selected in as input parameters in the "dimensio_reduction" function.

## Acknowledgements

Palle Steen Helmke provided the cholestasis dataset and assisted during development of the dimensionality reduction Jupyter Notebook.

ChatGPT [https://chat.openai.com/] was used to aid during code and README file documentation.

## License

Repository license: [LICENSE](./LICENSE)
