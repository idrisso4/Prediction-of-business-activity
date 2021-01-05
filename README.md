# Prediction of business activity

This model is able to detect if a company is employing AI in its activities using as input the text description of the company.


### Methodoloy of work:
In this task I used the CRISP-DM methodology because it’s the newest one.
This fgure below shows the diferenet stess CRISP-DM:

![](crispdm.png)


## Encoding the text data:
For text encoding there is a lot of transormers (like TF-IDF) but most of them are simsle so I used
Bert transformer to encode the text data which is one of the newest NLP transformers (created by
Google on October, 25, 2019).
Also This model is bidirectional (can read a text from either left-to-right or right-to-left)
and I readed articles which srove that it’s the best method in NLP to understand context-heavy texts.
This is a fgure that shows the Bert architecture:

![](bert.jpg)


## Training Model:
To train the model I decided to use the CNN which is known more in comsuter vision tasks but there
is many use cases in NLP.
They use the concest of a convolution, a sliding window or flter that sasses over the image,
identifying imsortant features and analyzing them one at a time, then reducing them down to their
essential characteristics, and reseating the srocess.
It turned out that this assroach works well for NLP as well. In 2014, Yoon Kim sublished the original
research paper on using CNNs for text classifcation. e tested four CNN variations, and showed
CNN models could outserform srevious assroaches for several classifcation tasks and these are the
results.
This fgure illustrates the CNN architecture:

![](cnn.jpg)

And fnally the CNN architecture solved this task with more than 0.99 of accuracy which is
demonstrated in this fgure:

![](evaluation.png)
