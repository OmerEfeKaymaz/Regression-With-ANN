# Regression with ANN

This project demonstrates the application of an Artificial Neural Network (ANN) for regression tasks using a butterfly image dataset. It provides an end-to-end pipeline from data preprocessing to model evaluation, showcasing the potential of deep learning in regression problems.

## Features
- **Image Preprocessing**: Resizing, color conversion, and feature extraction from butterfly images.
- **Feature Extraction**: Extracts top-left corner pixels for simplified model input.
- **ANN Architecture**: A feedforward neural network with fully connected layers, implemented using Keras.
- **Performance Metric**: Model evaluation with Mean Absolute Percentage Error (MAPE).

## Workflow
1. **Dataset Download**: Fetch the butterfly dataset from Kaggle.
2. **Data Preprocessing**: Load images, resize, and convert them for analysis.
3. **Feature Engineering**: Extract features from image matrices.
4. **Model Training**: Train the ANN with scaled data.
5. **Evaluation**: Evaluate the model's performance for each class.

## Requirements
- Python 3.8+
- Libraries: 
  - `pandas`
  - `numpy`
  - `cv2`
  - `keras`
  - `scikit-learn`
  - Kaggle API

Install the required libraries using:
```bash
pip install pandas numpy opencv-python keras scikit-learn kaggle
```

## How to Run
1. Download the dataset using Kaggle API:
```bash
kaggle datasets download -d phucthaiv02/butterfly-image-classification -p /content/
```
2. Extract the dataset and preprocess the images.
3. Open the `.ipynb` file in a Jupyter Notebook or Google Colab.
4. Run the cells step by step to train and evaluate the model.
5. Review the MAPE results for each class.

## Output Example
- Shape of processed image matrices: `(10, 30, 256, 256)`
- Extracted dataset shape: `(10, 30, 2, 2)`
- MAPE values for each class: 
```plaintext
Class                 Average MAPE
EASTERN DAPPLE WHITE  3.15
RED POSTMAN           2.96
MANGROVE SKIPPER      2.92
BLACK HAIRSTREAK      2.94
```

## License
MIT License

Copyright (c) 2024 Ömer Efe Kaymaz

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## Contributions
Contributions to improve the project or extend its functionality are welcome! Feel free to fork the repository and submit pull requests.

---

*Author: Ömer Efe Kaymaz*
