# Capstone Project 1: Anthropometric Data Analysis (NHANES 2020)

**Training:** Corizo Data Science Training  
**Project type:** Individual capstone project  
**Notebook:** `CapstoneProject1.ipynb`

## Project Overview

This project explores anthropometric measurements from adult male and female datasets associated with NHANES 2020. It uses Python for data loading, cleaning/inspection, statistical analysis, and visualization to compare body-measurement distributions and examine relationships between selected measurements.

## Objectives

The notebook covers the following tasks:

1. Retrieve the male and female datasets from GitHub.
2. Load the datasets into Pandas DataFrames and NumPy arrays.
3. Compare male and female weight distributions using histograms.
4. Compare weight distributions using boxplots.
5. Calculate descriptive statistics, including measures of central tendency, spread, and skewness.
6. Calculate Body Mass Index (BMI) for the female dataset.
7. Standardize female measurements using z-scores.
8. Explore relationships between standardized measurements using pairplots and Pearson/Spearman correlations.
9. Calculate waist-to-height ratio (WHtR) and waist-to-hip ratio (WHR).
10. Compare body-ratio distributions.
11. Discuss advantages and limitations of BMI, WHtR, and WHR.
12. Examine female participants with the lowest and highest BMI values.

## Technologies and Libraries

- Python
- Jupyter Notebook / Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Requests

## Repository Structure

```text
.
├── CapstoneProject1.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

The notebook downloads the source CSV files when its dataset-retrieval cell is run, so the CSV files do not have to be committed to this repository.

## How to Run

### Option 1: Google Colab (recommended)

1. Upload `CapstoneProject1.ipynb` to your GitHub repository.
2. Open [Google Colab](https://colab.research.google.com/).
3. Select **File → Open notebook → GitHub** and paste your repository URL, or upload the notebook from your computer.
4. Run the notebook cells from top to bottom.
5. Allow the dataset-retrieval cell to download the CSV files from the source repository.

The runtime needs internet access to download the datasets.

### Option 2: Run locally

1. Install Python 3.10 or later.
2. Clone or download this repository.
3. Open a terminal in the project directory and install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Start Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Open `CapstoneProject1.ipynb` and run the cells from top to bottom.

## Data Source

The notebook retrieves the male and female CSV files from the `gagolews/teaching-data` GitHub repository:

- [Male anthropometric dataset](https://raw.githubusercontent.com/gagolews/teaching-data/master/marek/nhanes_adult_male_bmx_2020.csv)
- [Female anthropometric dataset](https://raw.githubusercontent.com/gagolews/teaching-data/master/marek/nhanes_adult_female_bmx_2020.csv)

The notebook uses the measurements provided in these files. Please consult the original data source and its documentation for dataset definitions, sampling details, and permitted uses.

## Outputs

Running the notebook produces numerical summaries and visualizations, including:

- Histograms and boxplots comparing weight distributions
- Descriptive statistics and distribution-shape measures
- BMI calculations
- Standardized measurements (z-scores)
- Pairplots and Pearson/Spearman correlation matrices
- Waist-to-height and waist-to-hip ratio comparisons
- Comparisons of participants at the low and high ends of the female BMI distribution

## Important Notes

- Run the notebook cells in order because later sections depend on variables created earlier.
- The notebook downloads data from a remote GitHub URL, so the source must remain accessible and the runtime must have internet access.
- Statistical associations and anthropometric indices are exploratory; they should not be interpreted as individual medical diagnoses.
- The analysis and interpretations reflect the data and code in this notebook. Re-run the notebook to reproduce outputs in your own environment.

## Author

**Name:** Ahire Hrishikesh Bhaveshkumar
**Program:** Corizo Data Science Training  
**Project:** Capstone Project 1

> Before submitting, replace `[Your Name]` with your name and confirm that the notebook runs from top to bottom in a fresh Colab session.
