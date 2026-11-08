# Car Price Prediction

Final project of the 90-hour **Introductory AI & Data Science Course** (University of Kurdistan & Islamic Azad University of Sanandaj), September 2024. Three-person team; I led it.

- 🥇 **1st place** in the course project, with a scholarship
- Commended at **Research Week**, Islamic Azad University of Sanandaj (December 2024)

## Result
- **R² ≈ 0.97**: mean 8-fold cross-validation score of the final Random Forest pipeline (`final releas.ipynb`)

The event ranked teams by a combined score, ((1 − median absolute percentage error) + R²) / 2. An earlier version of this README called that score "accuracy"; it isn't, and R² is the number to quote.

## Approach
1. Clean the listings data and encode categorical features (title, transmission, body and interior colour, body status and type, …) with one-hot encoding; scale numeric features.
2. Train a **Random Forest** regressor in a scikit-learn pipeline, tuned with grid search and 8-fold cross-validation.
3. Compare with **HistGradientBoosting** and a small neural network.

## Files
- `first version.ipynb`: exploration and first models
- `final releas.ipynb`: final pipeline and submission

## Stack
Python · pandas · NumPy · scikit-learn · Matplotlib
