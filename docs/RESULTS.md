# Results

## Test performance

| Model | Accuracy | Precision | Recall | F1-score |
|---|---:|---:|---:|---:|
| VGG16 | 98.36% | 98.39% | 98.36% | 98.36% |
| Hybrid VQC | 97.82% | 97.89% | 97.82% | 97.83% |
| AlexNet | 95.64% | 95.69% | 95.64% | 95.64% |
| ResNet50 | 90.00% | 89.88% | 90.00% | 89.92% |
| Pure VQC | 80.22% | 81.01% | 80.22% | 79.70% |

## Interpretation

VGG16 gives the highest test accuracy in the executed experiment. The Hybrid VQC reaches 97.82%, showing that the quantum classifier can operate effectively on compact VGG16-derived features. The Pure VQC reaches 80.22% when working from PCA-reduced raw pixels.

The figures in this folder are extracted directly from notebook outputs.
