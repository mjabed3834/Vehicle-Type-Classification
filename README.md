---

# Vehicle Type Classification

This project aims to classify vehicle types using deep learning models. The dataset includes 7 classes of vehicle types, and various models have been employed to achieve accurate classification.

## Dataset

The dataset consists of images distributed across 7 classes:
- **Bike**
- **Couse Bus**
- **Micro Bus**
- **SUV**
- **Sedan Car**
- **Taxi**
- **Truck or Tanker**

### Data Distribution

- **Training Set**: 2498 images
- **Validation Set**: 988 images
- **Test Set**: 520 images

### Class Indices

```python
class_indices = {
    'Bike': 0,
    'Couse Bus': 1,
    'Micro Bus': 2,
    'SUV': 3,
    'Sedan Car': 4,
    'Taxi': 5,
    'Truck or Tanker': 6
}
```

## Models Used

The following models were employed for vehicle type classification:
- **Convolutional Neural Network (CNN)**
- **MobileNetV2**
- **InceptionV3**
- **DenseNet201**
- **Xception**
- **VGG16**

## Project Structure

```
Vehicle_Type_Classification/
├── data/
│   ├── train/
│   │   ├── Bike/
│   │   ├── Couse Bus/
│   │   ├── Micro Bus/
│   │   ├── SUV/
│   │   ├── Sedan Car/
│   │   ├── Taxi/
│   │   ├── Truck or Tanker/
│   ├── validation/
│   │   ├── Bike/
│   │   ├── Couse Bus/
│   │   ├── Micro Bus/
│   │   ├── SUV/
│   │   ├── Sedan Car/
│   │   ├── Taxi/
│   │   ├── Truck or Tanker/
│   ├── test/
│   │   ├── Bike/
│   │   ├── Couse Bus/
│   │   ├── Micro Bus/
│   │   ├── SUV/
│   │   ├── Sedan Car/
│   │   ├── Taxi/
│   │   ├── Truck or Tanker/
├── notebooks/
│   ├── Vehicle Type Classification.ipynb
├── models/
│   ├── cnn_model.h5
│   ├── mobilenetv2_model.h5
│   ├── inceptionv3_model.h5
│   ├── densenet201_model.h5
│   ├── xception_model.h5
│   ├── vgg16_model.h5
├── requirements.txt
└── README.md
```

## Setup and Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/Vehicle_Type_Classification.git
   cd Vehicle_Type_Classification
   ```

2. **Create a virtual environment and activate it:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. **Install the required packages:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Prepare the dataset:**
   - Ensure the dataset is placed in the `data/` directory following the structure provided above.

## Results

The results of the models will be saved in the `results/` directory. Each image file in this directory represents the performance metrics of a respective model.

The accuracies of the models are as follows:
- **CNN**: Accuracy: 0.9038
- **MobileNetV2**: Accuracy: 0.8269
- **InceptionV3**: Accuracy: 0.7865
- **DenseNet201**: Accuracy: 0.7808

## Conclusion

This project demonstrates the effectiveness of different deep learning models in classifying vehicle types. By leveraging state-of-the-art models, we can achieve accurate classification, which can be beneficial for various applications in the automotive industry and beyond.
