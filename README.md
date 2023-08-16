# Question Similarity with Siamese Neural Networks

## Objective

This project aims to build a system for learning question similarity using Siamese Neural Networks. The goal is to address the question retrieval task by identifying whether a given pair of questions is similar or dissimilar. This is particularly valuable in platforms like Quora and Stack Overflow, where users can benefit from finding existing answers to similar questions.

## Data

The project utilizes the Quora Question Pairs Dataset for training and testing the model. The dataset can be downloaded from [this link](http://qim.fs.quoracdn.net/quora_duplicate_questions.tsv).

## Architecture

The system's architecture is based on the MaLSTM (Manhattan LSTM) model as described in the paper cited in the references section. The overall architecture is depicted in Figure 1. While the paper discusses both English and Arabic languages, this project focuses on English question similarity.

![Figure 1: General architecture of the MaLSTM model](link_to_image)

## Implementation

The implementation is built upon the work conducted by the authors of the paper mentioned in the references. The Siamese Neural Network approach is used to learn question similarity. The model's performance can be extended and improved by incorporating your personal ideas and innovations.

## Usage

1. **Data Preparation**: Download the Quora Question Pairs Dataset from the provided link and preprocess it as necessary.

2. **Environment Setup**: Set up your Python environment with the required dependencies. You might find it helpful to create a virtual environment.

3. **Training**: Use the prepared dataset to train the Siamese Neural Network model. You can adjust hyperparameters, model architecture, and training strategies as needed.

4. **Evaluation**: Evaluate the trained model using appropriate metrics, such as accuracy, precision, recall, and F1-score.

5. **Inference**: Deploy the trained model to make predictions on new question pairs for similarity assessment.

6. **Extension**: Feel free to experiment with enhancements to the existing architecture, loss functions, or preprocessing techniques. Document your changes and results.

## References
[Manhattan Siamese LSTM for Question Retrieval in Community Question Answering](https://hal.science/hal-02271338/file/Manhattan_Siamese_LSTM_for_Question_Retrieval_in_Community_Question_Answering__1_.pdf)

