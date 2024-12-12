# Color Name to RGB Prediction Model

## Introduction
This project aims to develop a neural network model using Keras that can predict RGB color values from given color names. The model is built using character-level language modeling and incorporates both feed-forward and recurrent neural networks, specifically Long Short-Term Memory (LSTM) networks.

## Table of Contents
1. [Introduction](#introduction)
2. [Installation](#installation)
3. [Usage](#usage)
4. [Features](#features)
5. [Dependencies](#dependencies)
6. [Data Preparation](#data-preparation)
7. [Model Architecture](#model-architecture)
8. [Training](#training)
9. [Prediction](#prediction)
 

## Installation
To run this project, you need to have Python installed along with the following libraries:
- numpy
- scipy
- matplotlib
- tensorflow
- keras

You can install these dependencies using pip:
```bash
pip install numpy scipy matplotlib tensorflow keras
```

## Usage
Follow these steps to use the model :

  1. Data Preparation : Prepare your dataset of color names.

  2. Tokenization and Encoding : Tokenize the color names and encode them using one-hot encoding.

  3. Model Training : Train the model using the prepared data.

  4. Prediction : Use the trained model to predict RGB values from color names.

## Features
 1. Character-level language model for text input
 2. Uses LSTM networks for handling sequential data
 3. One-hot encoding for input representation
 4. Predicts RGB values normalized between 0 and 1
    
## Dependencies

   1. Python 3.x
   2. numpy
   3. scipy
   4. matplotlib
   5. tensorflow
   6. keras
      
## Data Preparation

   The color names are limited to 25 characters. Each character is tokenized and converted into an integer using Keras' Tokenizer utility. These integers are then padded and one-hot encoded for the model input.
  
   ![image](https://github.com/user-attachments/assets/d54848a1-b729-4196-aa0f-541f06078db2)
   
## Model Architecture

The model is built using Keras' Sequential API. It includes LSTM layers and dense layers with ReLU and sigmoid activations.
The color names are limited to 25 characters. Each character is tokenized and converted into an integer using Keras' Tokenizer utility. These integers are then padded and one-hot encoded for the model input.

![image](https://github.com/user-attachments/assets/cf390068-9661-44c9-adf3-f066d645557e)

## Training

The model is trained for 40 epochs with a batch size of 32. 10% of the data is reserved for validation to monitor overfitting.
  
## Prediction

To predict the RGB values from a color name, the input name is tokenized, padded, one-hot encoded, and then passed to the trained model.

![image](https://github.com/user-attachments/assets/bd6365bc-fd9c-406e-9136-a68bbe68ca4f)

 

