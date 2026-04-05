# VGG16 Image Classification

Binary image classification using VGG16 pretrained on ImageNet with a custom classification head. Built with TensorFlow/Keras.

---

## Dataset
- Cats vs Dogs via TensorFlow Datasets
- 5,000 training / 1,000 validation / 500 test images
- Resized to 150×150, preprocessed with VGG16 normalization

---

## Model
- **Base:** VGG16 pretrained on ImageNet (frozen)
- **Custom head:** GlobalAveragePooling2D → Dense(128, ReLU) → Dense(1, sigmoid)

---

## Results

| Split | Accuracy |
|---|---|
| Validation | 96.60% |
| Test | 96.40% |

---

## Notes
Training accuracy is higher than test accuracy, indicating overfitting.

---

## Tech Stack
Python, TensorFlow/Keras, TensorFlow Datasets

---

## Files
- `cats_vs_dogs_vgg16.ipynb`
- `README.md`
