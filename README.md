# Fashion-MNIST Clothing Classification with CNN
This project uses a Convolutional Neural Network (CNN) to classify clothing images from the Fashion-MNIST dataset using PyTorch.




## Objectives
- Understand the fundamentals of deep learning.
- Build an image classification model using CNN.
- Evaluate model performance on unseen test data.
- Analyze incorrect predictions.




## Tech Stack
- Python
- PyTorch
- Torchvision
- Matplotlib
- Google Colab


  

## Dataset used
Fashion-MNIST contains 70,000 grayscale images across 10 clothing categories.
- Training images: 60,000
- Test images: 10,000
- Image size: 28 × 28 pixels
- Number of classes: 10
  



## Model Architecture
- Convolutional Layer
- ReLU Activation
- Max Pooling
- Fully Connected Layers
- 10-class output




## Results
- Test Accuracy: 90.70%
- Correct Predictions : 9,070 / 10,000
- Training Epochs: 5




## Error Analysis
- The model sometimes misclassified visually similar clothing items.
- Examples observed :
  - Shirts were sometimes classified as T-shirts.
  - A sneaker was classified as a bag
  - Coats and pullovers were sometimes confused
- One possible reason is that Fashion-MNIST images are small (28 x 28 pixels), making some clothing details difficult to distinguish.




## Future Improvements
- Compare different CNN architectures.
- Tune learning rate and batch size.
- Analyze class-wise accuracy and a confusion matrix.
