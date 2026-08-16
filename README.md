# Assignment

Deep Learning — Fully Connected Networks, CNN and Transfer Learning

## Completed Work

### Fully Connected Neural Networks

- Regression: `dl/01_FCNN_Regression.ipynb` predicts Bengaluru house prices after cleaning mixed-format area and room fields, encoding categories, scaling numerical inputs, and using a dense Keras regression model.
- Classification: `dl/02_FCNN_Classification.ipynb` predicts bank customer churn with leakage-safe preprocessing, balanced class weights, and a binary dense Keras model.

### CNN

- Fashion-MNIST: `cnn/01_CNN_Fashion_MNIST.ipynb`
- CIFAR-10 with data augmentation: `cnn/02_CNN_CIFAR10.ipynb`
- Local directory image dataset: `cnn/03_Transfer_Learning_Local_Dataset.ipynb`

### Transfer Learning

- Pretrained model: MobileNetV2 with ImageNet weights
- Dataset: TensorFlow flower photos (five classes), reproducibly downloaded and extracted into class directories by the notebook
- Workflow: frozen feature extractor, new classification head, then low-learning-rate fine-tuning of the final layers

## Run in Google Colab

1. Open a notebook from GitHub with Google Colab.
2. For the two tabular notebooks, keep the CSV files in `labs/dl`; each notebook also includes a raw GitHub URL fallback.
3. Select a GPU runtime for the CNN notebooks (`Runtime` → `Change runtime type` → `T4 GPU`).
4. Run all cells from top to bottom. TensorFlow downloads Fashion-MNIST, CIFAR-10, flower images, and MobileNetV2 weights automatically when first needed.

All notebooks set `SEED = 42`, use moderate epoch limits, and use early stopping where helpful. Large downloaded image datasets and trained model files are not committed.

The committed outputs are real executions. The tabular notebooks used their complete supplied datasets. The CNN outputs were produced locally with `ASSIGNMENT_FAST_RUN=1` (reduced Fashion-MNIST/CIFAR-10 samples and epochs, but the same model logic); normal Colab execution uses the full default settings.
