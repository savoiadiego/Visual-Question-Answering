# Visual Question Answering
This was the third homework of the Artificial Neural Networks and Deep Learning course 2020/2021. All the details can be found on the [Kaggle inClass Competition page](https://www.kaggle.com/c/anndl-2020-vqa).

Developed by Diego Savoia and Francesco Emanuele Stradi.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/savoiadiego/Visual-Question-Answering/blob/main/Visual%20Question%20Answering.ipynb)

The goal was to solve a visual question answering (VQA) problem on the proposed dataset. The dataset is composed by synthetic scenes, in which people and objects interact, and by corresponding questions, which are about the content of the images. Given an image and a question, the goal is to provide the correct answer. Answers belong to 3 possible categories: 'yes/no', 'counting' (from 0 to 5) and 'other' (e.g. colors, location, ecc.) answers.

### Implementation
The notebook is meant to be used in Google Colaboratory, loading the dataset from Drive as explained inside the notebook.
After the data preparation part, there are three different models to train and use for predictions:
* Custom model
* Custom model variation
* Transfer Learning using VGG-16

Every model can be trained on the given dataset, using 30% of the samples for validation. Then, the prediction can be computed on the samples in the test folder. After that, the csv file containing the predictions is exported inside the Drive directory.
