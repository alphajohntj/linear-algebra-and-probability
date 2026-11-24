# Wine Quality – Linear Algebra and Probability

## Project overview
This project analyzes the supplied red wine quality dataset using Python, Pandas, NumPy, Matplotlib, and Seaborn. It covers missing-value handling, vector extraction, covariance, eigen decomposition, and empirical probability.

## Dataset
- File: `winequality-red.csv`
- Shape: 1,599 rows × 12 columns
- Target: `quality`
- Features include alcohol, citric acid, density, acidity, residual sugar, pH, sulphates, and others.

**Note:** The supplied file is the red wine dataset, not a combined red-and-white wine dataset.

## Tasks covered
1. Replace missing numeric values with their respective column means.
2. Extract `alcohol` and `citric acid` as NumPy vectors.
3. Calculate the covariance matrix for `alcohol` and `density`.
4. Perform eigen decomposition and interpret the two eigenvalues/eigenvectors.
5. Identify the most common quality score and examine its empirical distribution.

## Main findings from the supplied CSV
- No missing values were present.
- The most common quality score is **5** (681 samples; approximately 42.59%).
- Quality score **6** appears 638 times (approximately 39.90%).
- Scores 5 and 6 together represent approximately 82.49% of the samples.
- The alcohol–density covariance matrix is approximately:

```text
[[ 1.13564740e+00, -9.97951790e-04],
 [-9.97951790e-04,  3.56202945e-06]]
```

- The largest eigenvalue is approximately `1.13564827`; the second is approximately `0.0000026851`.
- The largest-eigenvalue direction is almost aligned with alcohol because the features are not standardized and alcohol has a much larger raw variance than density.

## Files
- `Wine_Quality_Linear_Algebra_Probability.ipynb` – documented notebook with code and visualizations.
- `winequality-red.csv` – original dataset.

## How to run
1. Install Python and Jupyter Notebook.
2. Install dependencies: `pip install pandas numpy matplotlib seaborn`
3. Keep the CSV and notebook in the same folder.
4. Open the notebook and run all cells.

## Tools
Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook.
