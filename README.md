# Assignment

Deep Learning — Fully Connected Networks, CNN, and Transfer Learning

## Completed Work

### Fully Connected Neural Networks

- **Regression:** `dl/01_FCNN_Regression.ipynb` predicts Bengaluru house prices using data cleaning, feature preparation, and a dense Keras regression model.
- **Classification:** `dl/02_FCNN_Classification.ipynb` predicts bank customer churn using preprocessing, class weights, and a dense Keras classification model.

### CNN

- **Fashion-MNIST:** `cnn/01_CNN_Fashion_MNIST.ipynb`
- **CIFAR-10 with data augmentation:** `cnn/02_CNN_CIFAR10.ipynb`
- **Local image dataset:** `cnn/03_Transfer_Learning_Local_Dataset.ipynb`

### Transfer Learning

- Uses **MobileNetV2** with ImageNet weights.
- Uses the TensorFlow flower dataset with five classes.
- The model starts with frozen pretrained layers and a new classification layer, followed by fine-tuning of the final layers.

## Run in Google Colab

1. Open any notebook from GitHub using Google Colab.
2. For the tabular notebooks, keep the CSV files in the `dl` folder.
3. For CNN and transfer learning notebooks, select a GPU runtime:
   `Runtime → Change runtime type → T4 GPU`
4. Run the notebook cells from top to bottom.

TensorFlow will automatically download datasets such as Fashion-MNIST, CIFAR-10, and the flower dataset when required.

The notebooks use `SEED = 42` for consistent results and early stopping where appropriate. Large datasets and trained model files are not included in the repository.

The notebooks were run and tested with the provided datasets. Some CNN outputs in the GitHub versions use smaller sample sizes and fewer epochs to reduce execution time, while the normal Colab versions can be run using the full settings.
