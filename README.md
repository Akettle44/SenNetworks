# SenNetworks
Submission for Kaggle competition Hacking the Human Vasculature in 3D

## Required packages
 - Numpy
 - cv2
 - matplotlib
 - torch
 - torchvision
 - pandas
 - sklearn
 - tqdm

### Running UNET
The sample data conting 5 training images and 5 test images is already present. Only need to run the `unet.ipynb` notebook.

### Running Segformer + Segment Anything (Assuming just testing)
1. Ensure that you have the data folder with 6 images and 6 labels at the inner-most level
2. Enable your conda environment or python virtual env, open transformers.ipynb

#### Segformer:
1. Run the packages cell
2. Run the dataset cell
3. Run the 'ingest data' cell, shape should be (6,) for both
4. Run the split cell
5. Run the dataset / dataloader cell
6. Optional: Run sanity check cell
7. Run custom loss cell
8. Run Segformer custom cell
9. Scroll down to model load cell (after save cell), run it
10. Run decode cell
11. Run test cell, should observe results below

#### SAM:
1. Run all SAM cells, observe output at bottom