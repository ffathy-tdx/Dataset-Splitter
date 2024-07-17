# Dataset-Splitter
## Description
This project contains a script to process and split an image dataset into training and validation sets. The script reads metadata and annotations, then organizes the images and corresponding annotations into separate directories for training and validation. Initially, the script was used on the FSOCO dataset, but it can be edited to work with other datasets as needed.

## Modify the script (if necessary):
Adjust paths and parameters in the script as needed. You can change the 70% split variable to whatever percentage you want by modifying the train_cap value in the code.

## Features
- Reads metadata from a JSON file.
- Filters and processes images based on specific criteria.
- Copies images and their annotations into designated directories.
- Computes bounding box sizes for annotations.
- Splits data into training and validation sets based on a predefined ratio.

## Ensure the dataset follows this file structure
```
├── sampledata/
│   ├── meta.json
│   └── <subdirectories>/
│        ├── img/
│            └── <image files>
│        ├── ann/
│            └── <annotation files>
│
```
## Output
The processed images and annotations are saved into two main directories:
- fsoco/train: Contains training images and annotations.
- fsoco/val: Contains validation images and annotations.
