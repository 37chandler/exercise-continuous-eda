# Exercises: Exploring Numerical Data (IMS Chapter 5) and Pandas Basics

This in-class exercise explores techniques for visualizing and summarizing **numerical** data, following the material in *Introduction to Modern Statistics* Chapter 5.

## Learning Objectives

By completing this exercise, you will practice:
- Understand the basic functions of Pandas
- Creating and interpreting scatterplots, including LOWESS trend lines
- Visualizing distributions with dot plots, histograms, and density plots
- Computing and interpreting the mean, variance, and standard deviation
- Summarizing distributions with box plots, the median, quartiles, and IQR
- Understanding robust vs. non-robust statistics
- Applying log transformations to skewed data

## Data Setup

The data files available for download from Canvas. The zip file has `loan50.csv` and `county.csv` in it. You'll need the `car_listings.csv` data set we've been working with. 

Your repository structure should look like:
```
631-exercise-cts-eda/
├── README.md
├── exercise-pandas-overview.ipynb
├── exercise-pandas-overview-solutions.ipynb
├── exercise-exploring-numerical-data.ipynb
├── exercise-exploring-numerical-data-solutions.ipynb
├── car_listings.csv
├── loan50.csv
└── county.csv
```

## Notebooks

- **`exercise-pandas-overview.ipynb`** — We'll use this workbook first. This code provides reminders on Pandas techniques we've seen in reading and assignments. I've also called out a few steps in Assignment 1 that were tricky for people. Work through this notebook a bit during class, finishing afterward if needed. Some examples are completed for you, others you'll complete on your own.
- **`exercise-pandas-overview-solutions.ipynb`** — Complete solutions for reference.
- **`exercise-exploring-numerical-data.ipynb`** — Work through this notebook a bit during class, finishing afterward. Some examples are completed for you, others you'll complete on your own.
- **`exercise-exploring-numerical-data-solutions.ipynb`** — Complete solutions for reference.

## Topics Covered in Numerical EDA

### Part 1: Scatterplots
- **Basic scatterplots** — visualizing relationships between two numerical variables
- **LOWESS trend lines** — revealing nonlinear patterns with locally-weighted regression

### Part 2: Dot Plots and the Mean
- **Dot plots** — one-variable scatterplots for small datasets
- **Sample mean** — computing $\bar{x}$ manually and with pandas

### Part 3: Histograms, Density Plots, and Shape
- **Histograms** — binned counts for distributional shape
- **Density plots** — smoothed KDE curves
- **Shape description** — skewness, modality (unimodal, bimodal, multimodal)

### Part 4: Variance and Standard Deviation
- **Sample variance** $s^2$ — computing step by step and with pandas
- **Standard deviation** $s$ — interpretation and verification

### Part 5: Box Plots, Quartiles, and the Median
- **Box plots** — five-number summary and outlier detection
- **Five-number summary** — min, Q1, median, Q3, max
- **IQR** — interquartile range as a measure of spread
- **Side-by-side box plots** — comparing distributions across groups

### Part 6: Robust Statistics
- **Median and IQR** vs. **mean and standard deviation** — sensitivity to extreme values

### Part 7: Transforming Data
- **Log transformations** — making right-skewed distributions more symmetric
- **Transformations in scatterplots** — revealing hidden structure

## Required Libraries

If you don't have all the libraries installed, you can typically install them at the command line with something like: 
```bash
pip install pandas numpy matplotlib seaborn statsmodels
```

Remember, you can create a new code cell in your notebook and run the above with an exclamation mark at the front to run it at the terminal. This is nice because it ensures the installation happens in your chosen Python kernel:

```bash
!pip install pandas numpy matplotlib seaborn statsmodels
```

## Getting Started

1. Open `exercise-exploring-numerical-data.ipynb` in Jupyter or VS Code
2. Follow along with the exercises, completing the sections marked with `# YOUR CODE HERE:`
3. Run each cell and examine the outputs
4. Refer to the solutions notebook if you get stuck

## Datasets

Datasets  from the [OpenIntro project](https://www.openintro.org/):

- **`loan50`** — A 50-loan sample from Lending Club with variables like `interest_rate`, `loan_amount`, `total_income`, and `grade`
- **`county`** — 3,142 US counties with demographic and economic variables like `unemployment_rate`, `median_hh_income`, `pop_change`, and `pop2010`

We also have our `car_listings.csv` data set. It's available for download on Canvas in Modules 1, 3, and 4.