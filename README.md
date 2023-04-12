[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/ymop5HUw)
# CMPSC 310 Activity 15

## Deadline: April 12 by 9:50am

## Assignment

 For this activity follow [Neural machine translation with a Transformer and Keras](https://www.tensorflow.org/text/tutorials/transformer).

## Submission

Submit completed Colab notebook showing generated output.

## Data
The data that was used in the tutorial is Portuguese-English translation datasetD. It was pre-processed by using the tokenize method to turn both
the English and Portuguese text into tokens. Each token could represent a sentence-piece, word, subword, or character. The program uses a function that splits the English token into two sequences, one for inputs and one for labels. Each input is shifted by one step so that at each input location the corresponding label is the id of the next token. This is done to train the model to predict the next word in the sequence.

A Transformer is a sequence-to-sequence encoder-decoder model. The transformer has many parts

The embedding and positional encoding layer:

The embedding layer maps each token in the input sequence to a dense vector of fixed size, The attention layers used throughout the model see their input as a set of vectors, with no order. So in order to give the model some way to identify word order. The positional layer gives the model information about the position of each token in the input sequence.

Add and normalize:

The purpose of this part is to  provide a direct path for the gradient and it ensures that vectors are updated by the attention layers instead of replaced while the normalization maintains a reasonable scale for the outputs.



