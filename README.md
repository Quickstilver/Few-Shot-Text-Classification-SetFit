# Few-Shot Text Classification with SetFit

This project aims to analyze the few-shot learning performance of SetFit on three distinct text classification datasets. 

SetFit, a state-of-the-art method for few-shot learning, is compared against a variant that does not fine-tune the pre-trained Sentence Transformer (ST).

## Project Highlights:

- Utilizes three text classification datasets for evaluating few-shot learning performance.
- Compares SetFit's performance against a baseline (SetFit without fine-tuning the pre-trained ST).
- Employs the small-text and datasets libraries for easy dataset handling and model creation.
- Leverages Hugging Face Transformers for pre-processing and tokenization.
- Applies an Active Learning strategy using Prediction Entropy as a query strategy for selecting uncertain samples.
- Presents the results in terms of train and test accuracy for each iteration of the active learning process.

## Key Components:

### Datasets:

- Toxic Conversations 50k
- Tweet Eval Stance Abortion
- Catalonia Independence (Spanish)

### Libraries and Dependencies:

- small-text[transformers]==1.3.0
- setfit>=0.5.0
- datasets
- matplotlib
- Hugging Face Transformers

## Main Steps:
- Load and preprocess the datasets.
- Create a balanced initial labeled set for active learning.
- Create SetFit classifiers using the small_text library.
- Implement an active learning loop with a query strategy based on Prediction Entropy.
- Evaluate and store the train and test accuracy for each iteration.


## Conclusions:
This project showcases a comprehensive approach to comparing few-shot learning methods on different text classification tasks. The results can be used to inform future improvements in SetFit or other few-shot learning techniques.
