# Predicting Crime Factors in Philadelphia Using Gradient Boosting and XGBoost

This repository contains Python code and analysis for predicting crime factors in Philadelphia using advanced machine learning techniques, specifically Gradient Boosting (GBM) and XGBoost. The study investigates the relationships between various socioeconomic factors and non-aggravated theft crime rates over the years 2013-2022. This analysis aims to provide valuable insights into the underlying drivers of crime in Philadelphia and potentially inform crime prevention strategies.

## Dataset

The dataset used in this analysis is sourced from two reputable government agencies:

* Philadelphia Police Department: Provided crime data, which encompassed reported incidents of burglary, auto-related thefts, theft from person, and retail theft.
* United States Census Bureau's American Community Survey (ACS): Provided socioeconomic data at the overall city level, including:
  * Family unemployment rate
  * Percentage of population below the poverty level who did not receive SNAP benefits
  * Overall poverty rate
  * Percentage of population over 25 years old without a bachelor's degree
  * Percentage of uninsured population

## Methodology

### Data Preprocessing

* All data was standardized by subtracting the mean and dividing by the standard deviation for each feature to improve the performance and interpretability of the machine learning models.

### Model Training and Evaluation

* Two models were trained and compared:
  * Gradient Boosting Machine (GBM): An ensemble learning method that builds sequential decision trees.
  * XGBoost: A highly optimized implementation of gradient boosting known for its efficiency and performance.
* Both models were evaluated using 10-fold cross-validation to assess robustness and generalization ability.
* The Root Mean Squared Error (RMSE) was used as the primary performance metric.

### Feature Importance Analysis

* Feature importances were calculated for both models to determine which socioeconomic factors are the strongest predictors of crime rates.

## Results

### GBM

* The GBM model predicts auto-related thefts most accurately (RMSE: 0.3943) and struggles the most with theft from person (RMSE: 0.8331).
* Educational attainment (No Bachelor's Degree Over Age 25) is the strongest predictor of theft across all categories.

### XGBoost

* The XGBoost model predicts burglary most accurately (RMSE: 0.5088) and struggles most with theft from person (RMSE: 0.9616).
* The key predictors of theft vary significantly across categories in the XGBoost model.

## Conclusions and Implications

Both GBM and XGBoost demonstrated their effectiveness in predicting crime rates using socioeconomic data. GBM specifically resulting in education attainment being the main factor in contributing to non-aggrevated crime. The results for XGBoost was varying. 

## Requirements

* Python 3.x
* Libraries: pandas, NumPy, scikit-learn, xgboost, matplotlib

## Usage

1. Clone this repository.
2. Install the required libraries using `pip install -r requirements.txt`.
3. Run the main script (`main.py`) to perform the analysis and generate the plots.
4. Explore the notebooks in the `notebooks/` directory for detailed code and explanations.

## Contributing

Contributions to this project are welcome. If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more information.

## Acknowledgments

* The dataset used in this analysis was obtained from The Philadelphia Police Department and the United States Census Bureau for the years 2013-2022.

## Contact

For any questions or inquiries, please contact rp955@drexel.edu




```python

```
