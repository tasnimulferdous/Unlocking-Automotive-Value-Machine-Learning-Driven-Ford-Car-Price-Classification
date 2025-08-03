# Unlocking Automotive Value: Machine Learning-Driven Ford Car Price Classification

## Project Overview
This project leverages advanced data analysis and machine learning to classify Ford car prices into Low, Medium, and High categories, utilizing features such as model, year, mileage, fuel type, and engine capacity. The framework delivers data-driven insights to empower automotive dealerships, buyers, and sellers with accurate, automated price predictions, enhancing inventory management and market research efficiency.

## Dataset
The dataset, sourced from Kaggle's "Ford Car Price Prediction" ([link](https://www.kaggle.com/datasets/adhurimquku/ford-car-price-prediction)), comprises 17,966 entries with nine features: `model`, `year`, `price`, `transmission`, `mileage`, `fuelType`, `tax`, `mpg`, and `engineSize`. It includes categorical (`model`, `transmission`, `fuelType`) and quantitative (`year`, `price`, `mileage`, `tax`, `mpg`, `engineSize`) variables, forming a robust basis for predictive modeling.

## Methodology
The project implements a comprehensive machine learning pipeline:
- **Data Preprocessing**: Handled missing values (e.g., imputed median for `tax`), removed outliers (e.g., years > 2025), and derived a new `age` feature to improve prediction accuracy.
- **Feature Engineering**: Applied one-hot encoding to categorical variables and used StandardScaler to normalize numeric features for non-tree-based models.
- **Model Selection**: Trained and evaluated four classification models:
  - Random Forest (89% accuracy)
  - PCA-Random Forest (86% accuracy)
  - Decision Tree (87% accuracy)
  - Logistic Regression (67% accuracy)
- **Evaluation**: Models were assessed using accuracy and macro F1-score, with Random Forest excelling due to its robust handling of complex feature interactions.

## Results
The Random Forest model achieved the highest accuracy of **89%**, demonstrating superior performance in classifying Ford car prices across all categories. Confusion matrices provide detailed insights into model performance, with Logistic Regression showing limitations in handling class imbalances for the High category.

## Repository Contents
- `code/`: Python scripts for data preprocessing, feature engineering, model training, and evaluation.
- `data/`: Link to the Kaggle dataset used in this project.
- `notebooks/`: Jupyter notebooks detailing exploratory data analysis (EDA) and model experimentation.
- `report/`: Comprehensive project report (`cse437ProjectReport.pdf`) outlining methodology, results, and future work.

## Dataset Link: 
https://www.kaggle.com/datasets/adhurimquku/ford-car-price-prediction


## Future Work
Future enhancements include hyperparameter optimization, incorporation of additional features (e.g., car condition, market trends), and exploration of advanced models such as Gradient Boosting to further improve accuracy.

## Authors
- Tasnimul Ferdous Tamim
- Asir Abrar Tonish
- Shamsan Nasir
- Sameer Khairul
- Supervised by Dr. Golam Rabiul Alam

*Department of Computer Science and Engineering, BRAC University, Dhaka, Bangladesh*

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments
We acknowledge Kaggle for providing the dataset and BRAC University for supporting this research. For further details, refer to the project report or contact us at {tasnimul.ferdous, asir.abrar.tonish, shamsan.nasir, sameer.khairul}@g.bracu.ac.bd.
