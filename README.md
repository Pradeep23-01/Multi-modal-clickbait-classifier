# Multi-modal-clickbait-classifier
A multimodal deep learning model that anticipates the clickbait nature through the text and images uploaded on social media, this study seeks to recognize social media posts in a heuristic manner

## Dataset: https://webis.de/data/webis-clickbait-17.html

# Context: 
Content that is written primarily to grab readers’
attention is referred to as clickbait. These enticing contents
encourage readers to click on links, which then direct them
to a certain web page. The goal of clickbait articles is not
to provide consumers with high-quality material but rather to
generate website traffic. It is crucial to ensure that the social
media updates made by digital marketing executives about newly
released news pieces are not clickbait. Through a multimodal
deep learning model that anticipates the clickbait nature through
the text and images uploaded on social media, this study seeks to
recognize social media posts in a heuristic manner. We train the
current state-of-the-art text classifiers and image classifiers on
our dataset, and the best-performing models for text and image
which are Bi-GRU and CNN respectively. These models were
considered to build the multimodal model, with the output based
on an output function.

# Results and Discussions: 
we proposed a Multimodal model for click-
bait detection on social media platforms that predicts both
the images and text data posted. Considering the different
configurations of word embeddings and classifier models of
the whole dataset, Bi-GRU models trained with Word2Vec
embedding outperformed all the other models in the classi-
fication of text and performs better than traditional machine
learning algorithms in clickbait-detection tasks. The 2-layer
CNN model outperforms the VGG Network for the given
dataset provided. The multimodal model generated from the
best-performing classifiers classifies the social media post in
an efficient manner.
