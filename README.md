# Wine Quality Dataset Analysis: Linear Algebra & Probability

This project applies Linear Algebra and Probability techniques in Python to analyze the chemical properties and quality ratings of 1,599 red wine samples from the UCI Machine Learning Repository.

## Project Tasks & Methodology
1. **Data Loading & Preprocessing:** Loaded the dataset using `pandas` and imputed missing values using column means.
2. **Vector Extraction:** Extracted `alcohol` and `citric acid` features as 1D NumPy arrays (vectors).
3. **Covariance Matrix:** Computed the covariance matrix between `alcohol` and `density` using `np.cov(X.T)` to measure joint variability.
4. **Eigen Decomposition:** Calculated the eigenvalues and eigenvectors of the covariance matrix using `np.linalg.eig()` to identify the directions of maximum variance.
5. **Probability & Distribution Analysis:** Determined the modal quality score and analyzed the probability distribution across all quality ratings.

## Key Findings
* **Covariance:** `alcohol` and `density` exhibit a slight negative covariance ($\approx -0.001$), indicating that higher alcohol content corresponds to slightly lower wine density.
* **Eigenvalues & Eigenvectors:** The top eigenvalue ($\approx 1.136$) captures nearly 100% of the variance, aligned almost entirely along the `alcohol` feature axis due to its wider scale compared to `density`.
* **Quality Distribution:** Quality score **5** is the most common rating ($42.59\%$), followed by score **6** ($39.90\%$), showing a bell-shaped distribution heavily concentrated around average quality.

## Technologies Used
* **Python 3**
* **NumPy** (Vector operations, covariance matrix, eigen decomposition)
* **Pandas** (Data loading, cleaning, frequency analysis)

## How to Run
1. Ensure `winequality-red.csv` is in the same directory as the notebook/script.
2. Install required libraries: `pip install numpy pandas`
3. Run the Jupyter Notebook or Python script to view all outputs.
