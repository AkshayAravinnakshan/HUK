# Engineer Challenge

This archive contains an engineering challenge for HUK-Coburg. The aim is to set an open task in which candidates can demonstrate their skills in the context of machine learning engineering. The actual solution is therefore just as interesting as the way to get there and the tools used.

## Task

Imagine you are working in a team together with *Data Scientists* (m/f/d) on a solution for the [Kaggle's Tweet Sentiment Extraction Competition](https://www.kaggle.com/c/tweet-sentiment-extraction). One of their colleagues is Chris Deotte and he proposes the solution in the notebook **model_training.ipynb**. The team agrees that this solution should be moved to a *fictional production environment*. This is your task. You will find the selected weights for the model in **weights_final.h5**.

Make the model available as a web service in the sense of a microservice.
The following points should serve as orientation:

- Creation of a Python script for the web service
- Encapsulation of the model inference in a Python module (OOP)
- Creation of a Dockerfile to host the solution
- Test concept of essential functionalities
- Determine the latency/request time of the web service and describe conceptually how this can be improved

## Notes

The **transformers** package comes from *[Huggingface](https://huggingface.co/)*.
The weights in **weights_final.h5** were created with *Tensorflow 2.7.0*.
The web service receives text and sentiment.
In response, it returns the words that express the sentiment of the text.
The code is not error-free.
