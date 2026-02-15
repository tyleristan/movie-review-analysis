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
│   ├── IMDB_Dataset.csv
│   └── reviews_with_severity.csv
│
├── SCRIPTS/
│   ├── eda_and_cleaning.py
│   ├── movie-review-testing.R
│   └── roberta_sentiment.py
│
├── OUTPUT/
│   ├── anova_extremity_length_group.csv
│   ├── log_transformed_review_length.png
│   ├── mean_extremity_by_length_group.pdf
│   ├── pairwise_extremity_length_group.csv
│   ├── q_q_plot.png
│   ├── raw_review_length.png
│   └── t_test_review_length_sentiment.csv
│
├── README.md
└── LICENSE
```
## Section 3: Instructions for Reproducing Results

### Step 1: Clone the Repository

```bash
git clone https://github.com/purplemorgy/movie-review-analysis
cd move_review_analysis
```

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

### Step 3: Install Packages

**Base Packages (Required)**

These packages are required to run data preprocessing and exploratory data analysis:

```bash
pip install pandas matplotlib numpy statsmodels
```

**RoBERTa Sentiment Model (Optional)**

If you want to compute sentiment severity using the RoBERTa model instead of reading in the data from a csv, run:

```bash
pip install torch torchvision torchaudio transformers tqdm
```

---

### Step 4: Run Data Cleaning and Exploratory Data Analysis Script

Run this script to clean the IMDB dataset, generates EDA plots, and saves a cleaned dataset as cleaned_reviews.csv:

```bash
python SCRIPTS/eda_and_cleaning.py
```

---

### Step 5: Run Data Cleaning and Exploratory Data Analysis Script (Optional)

This step is optional. The core analysis can still be performed without running the RoBERTa model. Run this script to compute sentiment severity scores using RoBERTa:

```bash
python SCRIPTS/roberta_sentiment.py
```

---

### Step 6: Run the Hypothesis Testing Script

Run this script to perform analysis:

```bash
python SCRIPTS/movie_review_testing.R
```



