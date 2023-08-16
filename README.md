# Question Similarity with Siamese Neural Networks

## Objective

This project aims to build a system for learning question similarity using Siamese Neural Networks. The goal is to address the question retrieval task by identifying whether a given pair of questions is similar or dissimilar. This is particularly valuable in platforms like Quora and Stack Overflow, where users can benefit from finding existing answers to similar questions.

## Data

The project utilizes the Quora Question Pairs Dataset for training and testing the model. The dataset can be downloaded from [this link](http://qim.fs.quoracdn.net/quora_duplicate_questions.tsv).

## Notebooks

### Initial Analysis

In the initial analysis notebook, you performed an overview of the project and dataset. Here are some key findings:

#### Model Description

- Input: Two free-text fields, presumably questions.
- Output: A similarity score between 0 and 1, indicating the degree of similarity between the questions.

#### Dataset Description

- 400k question pairs.
- 150k examples of duplicate questions.
- 250k examples of non-duplicate questions.
- 350k distinct questions - some questions are frequently repeated.

### Main Code

In the main code notebook, you implemented the core components of your project. Here's a breakdown of the major sections:

#### Part 1: Preprocessing Text

The text preprocessing steps include:

1. Changing all words to lowercase.
2. Cleaning punctuations and translating abbreviations.
3. Tokenizing the words.
4. Removing stop words.
5. Removing numbers.
6. Creating a dictionary of unique words and their corresponding numbers.

#### Part 2: Preparing Embedding Layer and Model

In this part, you prepared the embedding layer and defined the Siamese Network architecture. You used a pre-trained GloVe embedding layer to convert words into 300-dimensional vectors. The architecture involves:

- Input layers for question pairs.
- Embedding layers with pre-trained embeddings.
- Bidirectional LSTM layers for both questions.
- Dot layer for cosine similarity.
- Batch normalization and dropout layers.
- Dense layers for prediction.

![Siamese Network Architecture](https://drive.google.com/uc?export=view&id=1avcV308SuphZXLO0-8aatgIh0dL76vBe
)

#### Part 3: Training the Model

You trained the Siamese Network model for 5 epochs, achieving a validation accuracy of approximately 82.36%. The training involved optimizing the model using the Binary Cross-Entropy loss function.

## Usage

1. **Initial Analysis**: Review the findings and insights from the initial analysis notebook to understand the dataset and project requirements.

2. **Main Code**: Follow the steps in the main code notebook to preprocess text, prepare the embedding layer, define the Siamese Network architecture, and train the model.

3. **Model Evaluation**: Assess the model's performance on your specific problem and dataset. Experiment with hyperparameters and architectures for potential improvements.

4. **Inference**: Use the trained model for predicting the similarity of new question pairs.


## References
[Manhattan Siamese LSTM for Question Retrieval in Community Question Answering](https://hal.science/hal-02271338/file/Manhattan_Siamese_LSTM_for_Question_Retrieval_in_Community_Question_Answering__1_.pdf)

