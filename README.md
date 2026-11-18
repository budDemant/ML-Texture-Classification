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
## Technologies Used
- Python 3
- NumPy
- scikit-learn
- scikit-image
- ...

## Setup Instructions

### Prerequisites
- Python 3.7 or later
- ...

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
pip install -r requirements.txt
```

### 5. Run the Program

```bash
python main.py
```


## Getting Started
1. WIP

## Potential Extensions
- WIP 

## License
MIT License