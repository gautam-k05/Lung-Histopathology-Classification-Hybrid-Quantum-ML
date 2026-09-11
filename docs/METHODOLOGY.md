# Methodology

The project evaluates three classical CNNs and two quantum-learning pipelines.

## 1. Dataset and preprocessing

The notebook uses the lung subset of LC25000:

- `lung_aca`
- `lung_n`
- `lung_scc`

There are 15,000 images in total, split into 10,500 training, 2,250 validation and 2,250 test images.

CNN experiments use 224×224 RGB inputs. The Pure VQC experiment uses 64×64 RGB images, flattened to 12,288 pixel dimensions.

## 2. Classical models

AlexNet, VGG16 and ResNet50 are evaluated as classical baselines. VGG16 and ResNet50 use ImageNet-pretrained weights.

## 3. Hybrid VQC

VGG16 is used as a feature extractor. Its 512-dimensional representation is reduced to four PCA components and passed to a four-qubit Variational Quantum Circuit.

The hybrid circuit uses four layers and rotation/entanglement operations before producing a three-class output.

## 4. Pure VQC

The Pure VQC does not use CNN features. The 12,288-dimensional flattened image representation is reduced to eight PCA components and classified with an eight-qubit, six-layer VQC.

## 5. Evaluation

The notebook evaluates:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrices
- Normalized confusion matrices
- ROC curves
- Macro ROC-AUC
- Training/convergence behavior

The README and figures are derived from the executed notebook.
