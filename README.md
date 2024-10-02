# Programming Assignment 1: Data Preparation and Understanding

This repository contains the **Jupyter Notebook** for **Programming Assignment
1** for the Fall 2024 semester. The assignment involves working with the
**Stanford Dogs Dataset**, performing image processing, feature extraction, and
basic text processing on a multi-class dataset.

## Dataset

The **Stanford Dogs Dataset** can be found
[here](http://vision.stanford.edu/aditya86/ImageNetDogs/). The classes are:

1. n02088094-Afghan_hound
2. n02091467-Norwegian_elkhound
3. n02109961-Eskimo_dog
4. n02113978-Mexican_hairless

## Requirements

To run the notebook, you need to install the following Python libraries:

```bash
pip install -r requirements.txt
```

### `requirements.txt`

```text
numpy
pandas
matplotlib
Pillow
scikit-image
scikit-learn
jupyter
```

## Directory Structure

```bash
.
├── Dataset
│   ├── Images              # Folder containing dog class images
│   ├── Annotation          # XML annotations for bounding boxes
├── Processed_Images        # Processed images (cropped, resized, grayscale)
├── Grayscale_Images        # Grayscale images
├── train.json              # JSON file for text processing (tweets dataset)
├── README.md               # This README file
├── notebook.ipynb          # Main Jupyter Notebook for the assignment
```

## Results

- **Edge Histogram Comparison**: The notebook outputs the Euclidean, Manhattan,
  and Cosine distances between selected edge histograms.
- **PCA Visualization**: A 2D plot shows the separability of dog classes based
  on PCA-reduced edge histograms.
- **Text Processing**: PCA plots for token count and TF-IDF features display
  class separability in the tweet dataset.

## Running the Notebook

To run the notebook:

1. Open the terminal and navigate to the project folder.
2. Start Jupyter Notebook by running:

   ```bash
   jupyter notebook
   ```

3. Open `notebook.ipynb` in your browser and execute the cells in order.
