# Image Classification Web App Using ResNet50 with Flask and Docker

This project is an implementation of an image classification web app using Flask, which is capable of classifying various elements. It utilizes a pre-trained ResNet50 model available in the Keras library for image classification.

## Demo

https://github.com/thespectacular314/Image-classification-using-ResNet50-with-Flask-and-Docker/assets/155757417/72f48960-2587-474b-92cf-201c22386774

## How to Use the Web App

1. Upload an input image to the web app.
2. The app will classify the image using the pre-trained ResNet50 model.
3. The predicted class label and the probability of the prediction will be displayed.

## Prerequisites

- Docker Desktop
- Flask (installed within the Docker container)

## How to Run Locally

1. Clone this repository using Git.

2. Open a terminal and navigate to the project directory.

3. Build the Docker image: `docker build -t img_class .`

4. Run the Docker container and map the host port `5000` to the container port 5000: `docker run -d -p 5000:5000 img_class`

5. Open your web browser and visit `http://127.0.0.1:5000` to access the web app.

**Note:** Be patient during the first run, as the ResNet50 model needs to be downloaded. This process may take some time.

## How to Import the ResNet50 Model

To import the pre-trained ResNet50 model in your Python code, use the following syntax:

```python
from keras.applications.resnet50 import ResNet50
