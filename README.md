# Texture Image Classification

[CONCISE PROJECT DESCRIPTION IN PARAGRAPH FORM]

## Project Overview
- **Heading bullet**
  - Subheading bullet


## How It Works
1. **Load the KTH-TIPS2-b dataset**
   - WIP
2. **Splitting the data**
   - *GroupShuffleSplit*: Split by sample, not a standard random train_test_split
   - e.g. train on 3 samples, validate/test on remaining sample
3. **Label encoding**
   - *LabelEncoder* function maps 11 material names to integers 0-10
   - 
4. **LBP preprocessing and execution**
   - Convert images to grayscale
   - Compute normalized histogram (np.histogram?) of LBP codes (2D texture map --> 1D feature vector for scikit-learn)
   - 
5. **HOG preprocessing and execution**
   - WIP
6. **Feature caching**
   - Helper function for saving extracted feature matrices to disk (np.save, .npy data folder)
7. **Evaluation
   - Overall classification accuracy score
   - Per-class accuracy function
   - Confusion matrix plotting function
## Technologies Used
Software | Recommended Version
-------- | -------------------
Python | 3.14.x
pip | 26.3
numpy | 2.5.5
scipy | 1.18.1
scikit-learn | 1.9.1 
scikit-image | 0.26.0
matplotlib | 3.11.2
notebook | 7.6.5
ipykernel | 7.4.0

## Setup Instructions

### Prerequisites
- Python 3.14.x
- git
- venv

### 1. Clone the Repository
```bash
git clone https://github.com/budDemant/ML-Texture-Classification.git
cd ML-Texture-Classification
```

### 2. Create a Virtual Environment (Recommended)

A virtual environment keeps this project's dependencies isolated from other Python projects.

**Windows:**
```bash
python -m venv venv
venv\Scripts\activate
```
**macOS/Linux:**
```bash
python3 -m venv venv
source venv/bin/activate
```

### 4. Install Dependencies

Install the runtime dependencies:

```bash
python3 -m pip install --upgrade pip
pip install -r requirements.txt
```

Verify software installations

```bash
python3 -c "import numpy, scipy, sklearn, skimage, matplotlib, PIL; print('All dependencies installed successfully.')"
```


### 5. Download and Prepare the KTH-TIPS2-b Dataset

The KTH-TIPS2-b dataset is not included in the Git repository and must be downloaded separately.

https://www.csc.kth.se/cvap/databases/kth-tips/download.html

Locate the KTH-TIPS2-b dataset and download the color image archive (kth-tips2-b_col_200x200.tar).

Create a directory for the dataset in the project directory:

```bash
mkdir data && cd data
tar -xf kth-tips2-b_col_200x200.tar
```

### 6. Running Jupyter Notebook
Once all dependencies have been installed and while the virtual environment is active, launch Jupyter Notebook from the project folder directory:

```bash
jupyter notebook
```

## Getting Started
1. WIP

## Potential Extensions
- WIP 

## License
MIT License
