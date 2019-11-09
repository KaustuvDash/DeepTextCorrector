# DeepTextCorrector
In day to day life we make many grammartical mistakes writing english sentence.Here is the trained deep learning model which will automatically detect the small grammartical errors in the sentence and provide you error free sentence.
## Dataset
I collected the english sentence from https://tatoeba.org/eng/. It consists of around 100k sentences in english.
## Creation of dataset
- I will breifly explain how i created my own dataset.
- First i remove **'a'** randomly from 5% of sentences.Then removed **'an'** randomly from 5% of sentences.
- Then removed **'the'** randomly from 5% of sentences.Then applying **'than'** with **'then'** in random 5% of sentences.
- Then applying **'there'** with **'their'** in random 5% of senteces.
- Cleanded senteces are called "output" and pretubated sentences are called "input".
## Training
- Model training is through many to manay seq2seq model in deep learning around 50 epochs.
- Model preformed really well in train data,test data also.
## Examples
- **Example 1**
* Input English sentence: i am taller then you .
* Actual  Translation: i am taller than you .
* Predicted Translation:  i am taller than you .
- **Example 2**
* Input English sentence: frog came out of the water .
* Actual  Translation: a frog came out of the water .
* Predicted Translation:  a frog came out of the water .
- **Example 3**
* Input English sentence: at last , day has arrived for us to act .
* Actual  Translation: at last , the day has arrived for us to act .
* Predicted Translation:  at last , the day has arrived for us to act .
## Future Work
The model works preety well but sometimes it failed to output correct sentence for long sentences.Now i am using **self attention** to improve the model performance for long sentences.Stay tunned.
## References
- https://medium.com/@praneethbedapudi/deepcorrection-3-spell-correction-and-simple-grammar-correction-d033a52bc11d
- https://arxiv.org/pdf/1412.7449v3.pdf
- http://atpaino.com/2017/01/03/deep-text-correcter.html
