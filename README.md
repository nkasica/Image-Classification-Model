# Image Classification Model

Image Classification is the process of analyzing pixel patterns in images in order to separate images into distinct classes. Utilizing the TensorFlow library and Keras API, I built my own image classification model in Python which can distinguish between images of cats and dogs with over 95% accuracy! 

## How it Works

Firstly, I began by downloading images to form a dataset. My entire dataset consists of 480 images, with a nearly equal split between images of cats and dogs. After removing unwanted images and shuffling the dataset to achieve a random ordering for my batches, I preprocessed the data by scaling each image to 256x256 pixels and created splits for training, validation, and testing data. Using a convolutional neural network, I trained my model on ~70% of the images, using the other ~20% for validation and the remainder for testing. If you take a look at the code, you can also see graphs of my model's accuracy and loss throughout the training process!

## Getting Started

### Dependencies
* TensorFlow version 2.16.1 - `pip install tensorflow`
* OpenCV version 4.9.0 - `pip install opencv-pthon`
* Matplotlib version 3.8.3 - `pip install matplotlib`
Note: If you want to be able to run this program on your computer's GPU, use `pip install tensorflow[and cuda]` instead

### Usage
You can load my trained model by downloading `catsanddogs.keras` from the "model" directory and import it using keras.models.load_model. Alternatively, you can download the code and play around with the model's parameters and datset to create new ones. You can easily train this model on any different binary dataset by replacing the directories in the "data" directory with you those of own images!
