# Product Image Classification with EfficientNetV2

This project classifies product images into 10 categories using deep learning with TensorFlow and Keras. The model employs EfficientNetV2 with transfer learning for improved accuracy.

## Project Structure
- `train_data/`: Training images (10 categories)
- `test_data/`: Test images (unlabeled)
- `product_classification.ipynb`: Project notebook
- `q1_submission.csv`: Predicted labels

## Approach
1. **Data Preparation:** Used `ImageDataGenerator` with augmentation (flips, shifts). Split into training and validation sets.
2. **Model:** EfficientNetV2 with frozen base layers and custom dense layers. Compiled with `Adam` optimizer and `categorical_crossentropy` loss.
3. **Training:** Applied `EarlyStopping` to prevent overfitting.
4. **Prediction:** Processed test images, predicted labels, and saved results to `q1_submission.csv`.

## Submission Format
The output `q1_submission.csv` contains:
| name                  | predicted |
|-----------------------|-----------|
| image1.jpg           | 10        |
| image2.jpg           | 5         |

