# Techdome

## NIKITA

## A023119820034


This is the solution for the assignment given by Techodome for the data scientist internship applicants. The problem states that a dataset is given with the dog images showing differnt emotions viz. sad, angry, relaxed and happy and a ML model is build, train and deployed.
The model is to be deployed in the form of an API using flask.


This code demonstrates how to use TensorFlow and Keras to train a MobileNetV2 model on the dataset you provided. The code uses data augmentation to generate new images for training, and adds a new top layer to the base MobileNetV2 model for classification. The code also sets up early stopping to prevent overfitting during training, and saves the trained model to an h5 file for later use.

Then, we create a Flask app instance and define a route for handling POST requests to the /predict endpoint. In this route function, we get the image from the request, preprocess it, make a prediction using the model, and return the prediction as a JSON object.

Finally, we run the app using the app.run() method.

Note: This code assumes that the trained model is saved in a file named dog_emotion_model.h5 in the same directory as app.py. Also, we have assumed that the input image size is 224x224. If your model requires a different input size, you may need to modify the code accordingly.
