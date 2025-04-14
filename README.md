# IMAGE-CLASSIFICATION-MODEL
COMPANY: CODTECH IT SOLUTIONS 

NAME: Aditya Nagare

INTERN ID: CT12WH88 

DOMAIN: Machine Learning

DURATION: 12 weeks 

MENTOR: NEELA SANTOSH

## DESCRIPTION OF TASK
Image Classification using CNN on CIFAR-10
This project is a beginner-friendly but powerful implementation of an image classification model using a Convolutional Neural Network (CNN) built with TensorFlow and Keras, trained on the CIFAR-10 dataset. The model learns to recognize and classify images into 10 different categories such as airplanes, cars, birds, cats, and more.


Tools and Libraries Used
1. TensorFlow and Keras
The core of this project is powered by TensorFlow, which is a widely-used open-source machine learning library developed by Google. It allows you to build and train deep learning models efficiently. We used Keras, a high-level API integrated with TensorFlow, which makes it easier to define models in a more human-readable way.

2. NumPy
We used NumPy to handle numerical operations and manipulate arrays, which is very useful when working with images as arrays.

3. Matplotlib
To visualize how the model learns over time, we used Matplotlib, a plotting library, to create graphs that show how accuracy and loss change during training.

## How It Works
1. Dataset Loading and Preprocessing
We used the CIFAR-10 dataset, which is included in TensorFlow’s datasets. This dataset contains 60,000 color images of size 32x32 pixels, across 10 different classes. The images are split into a training set (50,000 images) and a testing set (10,000 images).

The images are originally made up of pixel values from 0 to 255. We normalize these pixel values to a 0–1 range by dividing them by 255. This helps the model train faster and more accurately.

2. Model Architecture
The model is built using Keras’s Sequential API. It has the following layers:

Conv2D + ReLU Activation: Extracts features from the images using filters.

MaxPooling2D: Reduces the size of the image while retaining the most important features.

Another Conv2D + Pooling: Helps the model learn deeper and more abstract patterns.

Flatten: Converts the 2D feature maps into a 1D vector.

Dense Layers: Fully connected layers that help in decision-making.

Output Layer with Softmax: Outputs probabilities for each of the 10 classes.

3. Training the Model
We train the model using the Adam optimizer, which adjusts the learning rate automatically, and the sparse categorical crossentropy loss function, which is perfect for multi-class classification.

Training is done over 10 epochs, with 20% of the training data reserved for validation. During each epoch, the model updates its internal parameters to get better at predicting the correct labels.

4. Evaluating and Visualizing
After training, we test the model on the unseen test dataset to get the test accuracy. We also use Matplotlib to plot two graphs:

Accuracy over epochs (for both training and validation)

Loss over epochs

These plots help us understand if the model is learning correctly or overfitting.

5. Prediction and Visualization
To test the model's prediction ability, we take the first image from the test dataset, ask the model to predict its class, and then display the image with the predicted label using plt.imshow().

  ## Real-World Applications
This type of image classification model is widely used in many real-life scenarios, including:

Autonomous Vehicles: Recognizing objects like traffic signs, pedestrians, and other vehicles.

Healthcare: Classifying medical images like X-rays or MRI scans.

Retail: Automatically categorizing products in online stores based on images.

Agriculture: Identifying diseases in plants or categorizing crops.

Security: Facial recognition and surveillance applications.

   ## Where You Can Implement This
You can implement this project in several environments:

Jupyter Notebook / Google Colab: Great for quick prototyping with live visualization.

PyCharm / VS Code: For a more structured development experience.

Kaggle Kernels: If you want to share your work and use free GPUs.

 ## OUTPUT

 ![Image](https://github.com/user-attachments/assets/e44586c9-7391-4667-9cea-cf888dddbad9)

![Image](https://github.com/user-attachments/assets/ed5dba32-0dd0-4187-a86c-447973a83106)
Real-world apps: Once trained, you can deploy the model using TensorFlow Lite for mobile devices or use Flask/Django to serve it on the web.

## This project is a great introduction to deep learning with CNNs and TensorFlow. It shows how a simple neural network can be trained to understand and classify images — something that our brains do automatically, but machines must learn from scratch. By exploring and tweaking this model, you can build the foundation to create more advanced computer vision systems in the future.
