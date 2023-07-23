Generally auto encoders are used for Neural Machine Translation

We made use of attention in addition to autoencoders to study its effects on accuracy of translation

This model could be used for translation of other languages by providing appropriate data for training


Algorithm : 

Pass a sentence to encoder
Process sentence word by word
Maintain encoder state at every timestamp
Pass the all the states of the encoder to the intermediate module
Pass attention vector, states of encoder, translated sentence to decoder
Adjust the weights of decoder, attention vector, weights of encoder based on the passed output (actual translated sentence)
Dropout neurons based on dropout probability
Adam optimiser is used
