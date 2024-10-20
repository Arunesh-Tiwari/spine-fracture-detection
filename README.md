# Cervical Spine Fracture Classification using Deep Learning
View Complete Paper Here 👉 **https://link.springer.com/chapter/10.1007/978-981-97-5862-3_3**
#
This project presents a **computer-aided diagnosis system** for classifying cervical spine fractures using **deep learning models**. The system leverages **AlexNet** and **GoogleNet** architectures to identify and classify cervical spine injuries as **normal**, **fracture**, or **dislocation**. With an **accuracy of 99.67%**, the proposed model outperforms the average radiologist's accuracy, providing a reliable solution for assisting in the diagnosis of critical cervical spine injuries.

## Overview

Cervical spine fractures are often associated with severe consequences, such as paralysis or death. These injuries require timely and accurate diagnosis to prevent further complications. Our deep learning model is designed to assist doctors by automating the classification of cervical spine X-ray images, reducing human error and enabling quicker decision-making.
<p align="center">
  <img src="https://github.com/user-attachments/assets/3e1f03cf-0389-4dac-9833-3800dfac1851" alt="cervical spine pic">
</p>

<p align="center"><em>Figure 1: Cervical Spine X-ray Image</em></p>

The dataset used contains **772 cervical spine fractures** and **707 normal images**. Our model, trained using **AlexNet** and **GoogleNet** with transfer learning, classifies X-ray images into three categories: **normal**, **fracture**, and **dislocation**. The final accuracy achieved is **99.67%**, higher than the radiologists’ average accuracy of 90-95%.

## Key Features

- **Deep Learning Models**: AlexNet and GoogleNet are used for feature extraction and classification.
- **Saliency Maps**: Visualization of model attention to ensure explainability in the classification process.
- **High Accuracy**: Achieves an accuracy of **99.67%**, surpassing traditional radiological methods.
- **Transfer Learning**: Fine-tuning of pre-trained AlexNet and GoogleNet models for cervical spine classification.
- **Efficient Performance**: Designed to run on standard PCs or embedded systems with minimal setup.

## Methodology

1. **Dataset**: 
   - Images are divided into three categories: **normal**, **fracture**, and **dislocation**.
   - Preprocessing includes resizing images and converting them into a format suitable for AlexNet and GoogleNet input layers.
   - The dataset used for this project is available on Kaggle and contains:
      - **530 Cervical Spine Dislocation Images**
      - **772 Cervical Spine Fracture Images**
      - **707 Normal Images**

<p align="center">
  <img src="https://github.com/user-attachments/assets/57d341aa-e2cd-4abb-bec4-6b9496dd5c7f" alt="cervical spine pic">
</p>

<p align="center"><em>Figure 2: Dataset Sample Images</em></p>

2. **Model Architecture**:
   - **AlexNet**: Composed of five convolutional layers followed by three fully connected layers, using **ReLU** activations and **SoftMax** for final classification.
   - **GoogleNet (Inception)**: Utilizes different-sized convolutions (5x5, 3x3, 1x1) to capture multi-scale features.

3. **Training**:
   - Dataset is split into **70% training**, **15% validation**, and **15% testing**.
   - Optimization is done using **Stochastic Gradient Descent (SGD)** with a learning rate of 0.001 and scheduled annealing to prevent local minima.
   - Performance metrics include **accuracy**, **precision**, **recall**, **F1-score**, and **ROC curves**.

## Results

- **Model Performance**: Achieved **99.67% accuracy**, significantly higher than radiologists (92%).
- **Training**: The model was trained over **30 iterations** with each batch containing **10 samples**.
- **Saliency Maps**: Used to confirm the model's focus on key features of the X-rays that correspond to fractures or dislocations.

<p align="center">
  <img src="https://github.com/user-attachments/assets/8d20e336-f2f7-4ba1-bcc0-6011346c4788" alt="cervical spine pic">
</p>

<p align="center"><em>Figure 3: Confusion Matrix</em></p>

## Performance Metrics

| Metric        | Value       |
|---------------|-------------|
| **Accuracy**  | 99.67%      |
| **Sensitivity** | 76%       |
| **Specificity** | 97%       |
| **Precision**   | 99.6%     |
| **F1-Score**   | 99.6%      |


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
