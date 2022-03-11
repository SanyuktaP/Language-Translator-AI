# Language-Translator-AI
The objective of the project is to implement language translation model aka machine translation for converting German to English (and vice versa)

For this, the data is a text file (.txt) of English-German sentence
pairs. The actual data contains over 150,000 sentence-pairs.
However, it is suggested to use only the first 50,000 sentence
pairs to reduce the training time of the model.

You can download the Data set from
deu_eng.txt

1. Start off by defining our Seq2Seq model architecture:
● For the encoder, we will use an embedding layer and an
LSTM layer
● For the decoder, we will use another LSTM layer followed
by a dense layer
2. Use the RMSprop optimizer in this model as it’s usually a
good choice when working with recurrent neural networks.
3. Use ‘sparse_categorical_crossentropy ‘as the loss function.
This is because the function allows us to use the target
sequence as is, instead of the one-hot encoded
format. One-hot encoding the target sequences using
such a huge vocabulary might consume our system’s
entire memory
