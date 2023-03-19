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

# Word Embeddings:
Word embeddings are a type of natural language processing technique that represent words as vectors in a high-dimensional space, where similar words are closer together. Word embeddings are used in a variety of NLP tasks, including sentiment analysis, text classification, and machine translation. Word2Vec, FastText, and GloVe are some of the most popular algorithms for creating word embeddings.

- Word2Vec is a neural network-based algorithm that was introduced by Google in 2013. It learns the embeddings by training a neural network on a large corpus of text data. The model is trained to predict the probability of a word given its context or the probability of a context given a word. The embeddings are learned by optimizing the weights of the neural network.

- FastText, also developed by Facebook AI Research, is an extension of the Word2Vec model that incorporates subword information. Instead of representing words as atomic entities, FastText breaks words down into their constituent character n-grams, or subwords, and learns embeddings for these subwords. This approach is particularly useful for languages with complex morphology and allows for the learning of embeddings for rare words.

- GloVe (Global Vectors for Word Representation) is another algorithm for creating word embeddings that was developed by Stanford researchers in 2014. Unlike Word2Vec and FastText, which are based on neural networks, GloVe uses a matrix factorization technique to learn the embeddings. The algorithm works by constructing a co-occurrence matrix that captures the frequency of word co-occurrences in a large corpus of text. GloVe then factorizes this matrix to learn the embeddings.

In terms of performance, the choice between these algorithms often depends on the specific task and the characteristics of the text data. However, in general, Word2Vec and FastText are popular choices for tasks that require understanding the semantic relationships between words, while GloVe is often used for tasks that require understanding the global context of words in a corpus.

# Text Classifiers:
- BiGRU (Bidirectional Gated Recurrent Units) is a type of recurrent neural network (RNN) architecture commonly used for text classification tasks. BiGRU combines the forward and backward hidden states of a gated recurrent unit (GRU) in a bidirectional manner to improve the model's ability to capture context and dependencies in text data. The forward and backward hidden states are concatenated at each time step and passed through a fully connected layer to make a prediction.

- 1D CNN (Convolutional Neural Network) is a type of neural network architecture that is commonly used for image processing tasks, but it can also be used for text classification tasks. In text classification, a 1D CNN applies filters of different widths over the word embeddings to capture local patterns in the text data. The filters slide over the text data in a 1-dimensional fashion, and the resulting features are passed through a fully connected layer to make a prediction.

- Temporal Convolutional Neural Network (TCN) is a type of neural network architecture that is specifically designed for sequence modeling tasks, including text classification. TCN applies a series of convolutional layers to the sequence data, with each layer having a larger receptive field than the previous one. This allows the model to capture dependencies over longer time intervals in the sequence data. The output of the final convolutional layer is passed through a fully connected layer to make a prediction.

In terms of performance, the choice between these architectures often depends on the specific task and the characteristics of the text data. For example, BiGRU is useful for tasks that require capturing long-term dependencies and context in the text data. 1D CNN is useful for tasks that require capturing local patterns in the text data, such as sentiment analysis. TCN is useful for tasks that require capturing dependencies over longer time intervals in the text data.

# Results and Discussions: 
We proposed a Multimodal model for click-bait detection on social media platforms that predicts both the images and text data posted. Considering the different
configurations of word embeddings and classifier models of the whole dataset, Bi-GRU models trained with Word2Vec
embedding outperformed all the other models in the classification of text and performs better than traditional machine
learning algorithms in clickbait-detection tasks. The 2-layer
CNN model outperforms the VGG Network for the given
dataset provided. The multimodal model generated from the
best-performing classifiers classifies the social media post in
an efficient manner.
