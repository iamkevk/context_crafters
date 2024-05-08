# Fine-tuning Google's Gemma (7b) LLM with Kaggle-documentation synthetic dataset 

## Introduction
This exploratory project is the work for the group `Context Crafters` in the Georgia Tech Deep Learning graduate class (Spring 2024). Please visit this page for details of the [CS 7643](https://omscs.gatech.edu/cs-7643-deep-learning) class. 

***Disclaimer***: The views and opinions expressed in this project are those of the authors and do not necessarily reflect the views or positions of Georgia Tech.

## Project Overview

In February 2024, Google [released Gemma](https://blog.google/technology/developers/gemma-open-models/) Gemma, a family of lightweight open-source generative AI models, designed primarily for developers and researchers. Using Google's Gemma as the pre-trained model, we attempt in this project to fine-tune this foundation generative model to adapt it to perform better at question-answering content from [Kaggle documentation](https://www.kaggle.com/docs)  

## Motivation
In recent times the use of large language models (LLMs) for question-answering tasks has seen a significant increase, thanks to the impressive capabilities of models such as ChatGPT. However, foundation LLMs are not inherently adapted to domain-specific tasks and require some techniques to further train the model using a representative domain-specific dataset. The work in this project shows a possible approach for fine-tuning open-source language models to a specific task. 

## The problem

[Kaggle](https://www.kaggle.com/) is an online community for data science and machine learning (ML) that serves as a learning platform for both novices and seasoned professionals, offering realistic practice problems to sharpen data science skills. Currently, navigating its extensive documentation or forums can be daunting for many users, potentially limiting their ability to make the most of the platform. This project aims to illustrate the potential methods for developing an artificial intelligence (AI) assistant specifically tailored for Kaggle’s documentation. Potentially, the Question Answering Assistant can improve user experience significantly and reduce the workload of platform staff by providing immediate responses to user inquiries.

## The Challenge

The two ***primary challenges*** of fine-tuning a large language model faced by small businesses and individuals include:
- For effective fine-tuning, the training data must be of high quality, adequately large, and representative of the specific domain and task at hand.
- Fine-tuning large language models incurs additional expenses related to training and maintaining the specialized model.

We address these and more challenges of fine-tuning a large language model which can be a powerful technique to adapt LLMs to specific domains and tasks.

## Implementation Summary

- Foundation model used:  [Access Gemma on Hugging Face](https://huggingface.co/google/gemma-7b)
- Fine-tuning approach: [QLoRA-Quantized Low-Rank Adaptation](https://arxiv.org/abs/2305.14314)
- Computing environment: [V100 GPU](https://colab.research.google.com/notebooks/pro.ipynb)
- Dataset: Synthetic dataset generated from scrapped [Kaggle documentation](https://www.kaggle.com/docs) data
- Hyperparameter tuning: Please refer to the report for complete implementation details

## How to use

Please refer to 
- the [`report/Project_Report___CS_7643__Context_Crafters___Publish_Copy_.pdf`](https://github.com/iamkevk/context_crafters/blob/4e8a5cff5de62a3bf3cd9b5be5220cd832197a42/report/Project_Report___CS_7643__Context_Crafters___Publish_Copy_.pdf) and,
-  the accompanying [`notebook/QLoRA_Fine_Tuning_Gemma_Kaggle_Assistant.ipynb`](https://github.com/iamkevk/context_crafters/blob/0cdded452848311454d15260d492275dbd5dc03d/notebook/QLoRA_Fine_Tuning_Gemma_Kaggle_Assistant.ipynb)
-  The `datasets` are available for download [here](https://github.com/iamkevk/context_crafters/tree/f2f29c78997e681de0795cbcc82a92deba186d4e/dataset) 

### Authors

- Kevin Kori
- Krittaprot Tangkittikun
- James Mungai


## License

Please read the ***terms of use and licenses** for each of the above tools and datasets.



