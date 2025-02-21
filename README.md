# Breast Cancer Classification 🎗️

A deep learning project focused on classifying breast cancer based on diagnostic data. Early detection of breast cancer can significantly improve survival rates, and this project aims to contribute to this effort by building a machine learning model that can classify breast cancer cases based on various features.

## Table of Contents

- [Introduction](#introduction)
- [Why Breast Cancer Awareness is Important](#why-breast-cancer-awareness-is-important)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Output](#output)
- [Contributing](#contributing)
- [License](#license)
- 
## Introduction

Breast cancer is one of the most common types of cancer, especially among women. This project uses a dataset of diagnostic features to classify breast cancer as either benign or malignant. By leveraging machine learning and deep learning techniques, this model can assist medical professionals in identifying potential cancer cases with greater accuracy and efficiency.

## Why Breast Cancer Awareness is Important

1. **High Risk**: The average risk for women in the United States is approximately **13%**, which translates to a 1 in 8 chance of developing breast cancer.
2. **Health Impact**: Breast cancer can significantly impact one's life, potentially leading to changes in body shape, hair loss, early menopause, and loss of fertility.
3. **Importance of Early Detection**: Early detection of breast cancer can lead to better treatment outcomes, potentially saving lives.

## Dataset

![Dataset Sample](https://github.com/patelandpatel/Breast-Cancer-Classification/assets/129002378/8c840ccd-dc54-4814-ba0e-b31424cb325a)

The dataset used in this project contains diagnostic features for breast cancer cases, including attributes like radius, texture, perimeter, area, and smoothness of cell nuclei in biopsied cells. This information is used to classify each case as benign or malignant. The dataset can be found [here on Kaggle](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data) (or another link if applicable).

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/patelandpatel/Breast-Cancer-Classification.git
   cd Breast-Cancer-Classification
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Download the dataset and place it in the `data/` directory.

## Usage

1. **Preprocess the Data**  
   Run the data preprocessing script to clean and prepare the dataset for training:
   ```bash
   python preprocess_data.py
   ```

2. **Train the Model**  
   Train the breast cancer classification model:
   ```bash
   python train.py --dataset data/breast_cancer_data.csv --epochs 50 --batch_size 32
   ```

3. **Evaluate the Model**  
   Evaluate the trained model on the test dataset:
   ```bash
   python evaluate.py --model saved_model.h5 --test_data data/test_data.csv
   ```

4. **Predict on New Data**  
   Use the model to classify new samples:
   ```bash
   python predict.py --input path_to_input_data.csv --model saved_model.h5
   ```

## Output

![Output Sample](https://github.com/patelandpatel/Breast-Cancer-Classification/assets/129002378/1e454df1-4eff-4d10-ad7f-58dde1f55609)

The model outputs a prediction for each input case, classifying it as benign or malignant based on the diagnostic features. Accuracy, precision, recall, and other performance metrics are also available.

## Contributing

Contributions are welcome! If you have suggestions for improving the model or additional features, please consider contributing. Follow these steps:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-name`.
3. Commit your changes: `git commit -m 'Add a new feature'`.
4. Push to the branch: `git push origin feature-name`.
5. Create a pull request.

Please make sure to follow the [code of conduct](CODE_OF_CONDUCT.md) and adhere to the coding guidelines.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
