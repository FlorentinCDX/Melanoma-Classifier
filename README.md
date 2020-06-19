# Melanoma-Classifier

This prototype is available at the following address: https://skin-lesion-analyzer.000webhostapp.com/

## Motivation

The aim of this project is to assist dermatologists in making a diagnosis of a skin lesion. The tool returns the probabilities associated with the type of melanoma for a given skin lesion photo.The model is able to classify 7 types of skin lesions.

My goal for this project was to build an end to end solution - starting with model creation and ending with a live web app.
I used the HAM10000 Dataset on kaggle : https://www.kaggle.com/kmader/skin-cancer-mnist-ham10000 to train a CNN on a MobileNet database with transfer learning. I was able to obtain an accuracy rate of 82% on melanoma type recognition.
I then converted my model to TensroFlow.js to make it accessible as a webapp. I was able to create a website where users are able to submit a picture of a skin lesion and get an instant prediction.

The python code to build and train the model is included in the Jupyter notebook.

## How to use?

You just have to click on the button "Analyseur de lésions cutanées", select a picture of your skin lesion and within seconds the app will produce a result with the top three highest probability and the associated melanoma type.

## Features

I choose to train a MobileNet CNN because of it's light weight so that it can be load localy on a browser. To ensure privacy, user submitted images are pre-processed and analyzed locally and are never uploaded to an external server.

## Tech/framework used

* Python : TensorFlow, Keras, Pandas, Numpy, Scikit-Learn, Matplotlib
* HTML, CSS, Java-Script, tensorflowjs

You can check the entire model building and training in this Kaggle kernel : 
https://www.kaggle.com/florentincoeurdoux/classification-acc-82
