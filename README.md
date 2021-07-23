# Automatic-Essay-Scoring

A recurrent neural network method for determining the relationship between an essay and its grade. Using Long-Short Term Memory networks to represent the meaning of texts to demonstrate that a fully automated framework is able to achieve results. 

## Introduction:

The use of specialised computer systems to award grades to essays produced in an educational setting is referred to as automated essay scoring (AES). It is an application of natural language processing. Its goal is to sort a vast number of textual elements into a small number of discrete categories that correspond to various grades, such as 1 to 5. It can be considered a problem of statistical classification.

## Approach:

The system is built on recurrent neural networks, which can effectively encapsulate the information needed for essay evaluation and learn complicated patterns in data via non-linear neural layers. The link between the essays and evaluator ratings is discovered using machine learning techniques.

Recurrent neural networks have the potential to learn more complicated patterns from input and are theoretically more powerful. Long short-term memory units are recurrent units that have been improved to deal more efficiently with diminishing gradients. The information required for the final representation can be learned by LSTMs to be remembered or forgotten.

## Flow of the Notebook:

1. Importing Libraries and Dataset
2. Data Exploration
3. Feature Engineering
4. Topic Modelling
5. Building and Training the Model
6. Submission

### Feature Engineering:

#### i. Analyzing the top bigrams in our essay

<img src="https://github.com/geekquad/Automatic-Essay-Scoring/blob/main/assets/bigrams.png">

#### ii. WordCloud

<img src="https://github.com/geekquad/Automatic-Essay-Scoring/blob/main/assets/wordcloud.png">

### Topic Modelling:

Topic modeling is a group of unsupervised machine learning methods aimed to extract meaningful topics from a text corpus. Topic modeling is helpful in exploring a new text dataset and understanding the different types of text samples.

Using the Latent Dirichlet Allocation algorithm with 10 topics and print the most important words in every topic.

<img src="https://github.com/geekquad/Automatic-Essay-Scoring/blob/main/assets/modelling.JPG">



Over the training data, we apply the RMSProp optimization approach to minimise the mean squared error (MSE) loss function. In order to minimise overfitting, we also utilise dropout regularisation. We train the neural network model for a predetermined number of epochs and track its performance on the development set after each one.


## Refrences:

[1] [A Neural Approach to Automated Essay
Scoring](https://aclanthology.org/D16-1193.pdf), Kaveh Taghipour and Hwee Tou Ng.

[2] [Automatic Text Scoring Using Neural
Networks](https://arxiv.org/pdf/1606.04289.pdf), Dimitrios Alikaniotis, Helen Yannakoudakis
and Marek Rei.
