# movie-review-analysis

### Software Used
- Python (version 3.9 or higher)

### Python Packages Required

The following packages must be installed:

- pandas  
- matplotlib  
- numpy  
- torch  
- torchvision  
- torchaudio  
- transformers  
- statsmodels  

### Platform

This project was developed and tested on macOS.  
It should also run on Windows or Linux with the same Python setup.

## Section 2: Map of the Documentation

Project Folder Structure:

```
move_review_analysis/
│
├── DATA/
│   ├── reviews_with_severity.csv
│   └── IMDB_Dataset.csv
│
├── SCRIPTS/
│   └── movie-reviews-script.ipynb
│
├── OUTPUT/
│   ├── log_transformed_review_length.png
│   ├── q_q_plot.png
│   └── raw_review_length.png
│
├── README.md
└── LICENSE
```
## Section 3: Instructions for Reproducing Results

### Step 1: Clone the Repository

---

### Step 2: Create a Virtual Environment

Create a virtual environment:

```bash
python3 -m venv venv
```

Activate the virtual environment:

**Mac/Linux**
```bash
source venv/bin/activate
```

**Windows**
```bash
venv\Scripts\activate
```

---

### Step 3: Install Required Packages

Run this in your terminal:

```bash
pip install pandas matplotlib numpy torch torchvision torchaudio transformers statsmodels
```

---

### Step 4: Run the Analysis Script

Run the preprocessing and sentiment analysis script:

```bash
python SCRIPTS/movie_reviews_script.py
```

---

### Step 5: Run the Hypothesis Testing Script

After the first script completes, run:

```bash
python SCRIPTS/movie_review_testing.R
```



