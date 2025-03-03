# SMS Spam Detection using Gradio
=====================================

## Table of Contents
-----------------

* [Introduction](#introduction)
* [Step 1: Load the Dataset](#step-1-load-the-dataset)
* [Step 2: Preprocess the Data](#step-2-preprocess-the-data)
* [Step 3: Train the Model](#step-3-train-the-model)
* [Step 4: Create the Gradio App](#step-4-create-the-gradio-app)
* [Step 5: Test the App](#step-5-test-the-app)
* [Conclusion](#conclusion)

## Introduction
------------

This project uses Gradio to create a simple SMS spam detection app. The app uses a pre-trained pipeline with TF-IDF vectorization and Linear Support Vector Classification to classify SMS messages as spam or not.

## Step 1: Load the Dataset
-------------------------

* Load the `SMSSpamCollection.csv` dataset into a Pandas DataFrame.
* The dataset contains two columns: `text_message` and `label`.

## Step 2: Preprocess the Data
---------------------------

* Split the data into training and testing sets (67% for training and 33% for testing).
* Use TF-IDF vectorization to transform the text data into numerical features.

## Step 3: Train the Model
------------------------

* Train a Linear Support Vector Classification model on the training data.
* Use the trained model to make predictions on the testing data.

## Step 4: Create the Gradio App
-----------------------------

* Create a Gradio app with a text input box and a text output box.
* Use the trained model to make predictions on the user's input text.
* Display the prediction result in the output box.

## Step 5: Test the App
---------------------

* Test the app with the following text messages:
	1. You are a lucky winner of $5000!
	2. You won 2 free tickets to the Super Bowl.
	3. You won 2 free tickets to the Super Bowl. Text us to claim your prize.
	4. Thanks for registering. Text 4343 to receive free updates on medicare.
* Verify that the app correctly classifies the text messages as spam or not.

## Conclusion
----------

The Gradio app for SMS spam detection has been successfully created and tested. The app uses a pre-trained pipeline with TF-IDF vectorization and Linear Support Vector Classification to classify SMS messages as spam or not.
