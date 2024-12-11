# Dogs-vs-Cats-Classification-DL
This Python script processes a dataset of cat and dog images, performs image resizing, and trains a neural network model to classify the images. Here's a summary of the steps:

    Dataset Extraction and Setup: The script extracts a compressed dataset (Cats vs. Dogs) from a ZIP file and counts the number of images in each folder (cats and dogs).

    Image Preprocessing: It resizes all cat and dog images to 224x224 pixels and converts them to RGB format. Resized images are saved in new folders.

    Data Labeling: Labels are created for the images, with '0' representing cats and '1' representing dogs.

    Image Loading: The resized images are loaded into memory and prepared for training by combining the cat and dog image arrays and their corresponding labels.

    Data Splitting: The dataset is split into training and test sets, and the image pixel values are normalized by scaling them to a range of [0, 1].

    Model Building: A pre-trained MobileNetV2 model is used as a feature extractor in a simple neural network. A dense layer is added for classification.

    Model Training and Evaluation: The model is trained for 5 epochs, and its accuracy is evaluated on the test set.

    Prediction: The script provides a function to predict whether a given input image (provided by the user) represents a cat or a dog, displaying the result.

The model is evaluated on test data, and the accuracy is printed. Additionally, the user can input a path to an image for prediction, and the model will classify it as either a cat or a dog.
