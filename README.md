Return Prediction Project
Project Overview
This project focuses on predicting whether an order will be returned or not, based on historical order data. The dataset contains sales, refunds, and product details.

Dataset
The dataset used in this project is publicly available on Kaggle and contains transaction records including:

Category, Version, Buyer ID
Final Quantity, Total Revenue, Refunds
Refunded Item Count, Purchased Item Count
Date, Sales Tax, Overall Revenue
Data Preprocessing
Key preprocessing steps include:

Handling date features: extracting month, day of week, and weekend information.
Creating a target column is_returned based on negative quantities or refunds.
Encoding categorical features:
One-hot encoding for Category and day_of_week.
Frequency encoding for Version.
Undersampling the majority class to balance the dataset.
Model
A Random Forest Classifier is trained on the preprocessed data. Key parameters include:

n_estimators=200
max_depth=10
class_weight='balanced'
Results
After preprocessing and undersampling:

Accuracy: ~0.79
Confusion Matrix: [[1725, 166], [ 971, 2530]]
How to Use
Clone this repository.
Open the notebook return_prediction.ipynb in Jupyter or Kaggle.
Run the cells sequentially to reproduce the results.
Notes
The dataset is already publicly available on Kaggle.
No private or sensitive information is included in this repository.
Contributions are welcome!
