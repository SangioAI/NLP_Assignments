# NLP Assignments
[assignment1.ipynb](assignment1.ipynb) focuses on the creation of a full NLP pipeline to tackle the [EXIST 2023](https://clef2023.clef-initiative.eu/index.php?page=Pages/labs.html#EXIST) task on sexism identification in tweets using LSTM and Transformer -based models. Our approach consists of data pre-processing and models creation on which training and evaluations procedure are performed, with the help of the HugginFace library. We analysed the impacts of different architectural choices and discussed our classification performances, discovering that how we feed our data to the models play a crucial role in the final outcome.

[assignment2.ipynb](assignment2.ipynb) focuses on the implementation of open source Large Language Models (LLMs) with prompting approaches to tackle the task of detecting sexist in tweets. In this
report we will evaluate the classification performance and compare the performances of different pre-trained LLMs by using both zero- and few-shot-prompting techniques.

# Results
For more details look to [report1.pdf](report1.pdf) for assignment1 and [report2.pdf](report2.pdf) for assignment2.


Assignment 1 ([assignment1.ipynb](assignment1.ipynb))
----
In Table 1 are shown the best hyper-parameters searched via a hand-made2 GridSearch over number of LSTM layers (#L), the sexist output threshold (Thr.), the embedding dimension (Emb), the BCEWithLogitsLoss’s pos_weight or recall-precision importance factor (RPI), the learning rate (LR) and whether or not to apply a weighted loss on the batches (wL). The metrics used are F1 scores on validation (vF1) and test (tF1) sets.

<img width="272" alt="image" src="https://github.com/user-attachments/assets/2d18b300-b609-4b4a-bae9-cdb85d1e7077" />
Table 1: F1 scores of LSTM and Transformer models

Assignment 2 ([assignment2.ipynb](assignment1.ipynb))
----
In Table 2 inference on data is calculated for both of the models using the following configurations:
1. with zero-shot-prompting and temperature =
None (default value = 1)
2. with zero-shot-prompting and temperature =
0.3
3. with few-shot-prompting (number of exam-
ples per class = 2)
4. with few-shot-prompting (number of exam-
ples per class = 3)
5. with few-shot-prompting (number of exam-
ples per class = 4)

<img width="340" alt="image" src="https://github.com/user-attachments/assets/eca5aa54-7d19-41c9-a711-90e199734883" />
<em>Table 2: performance of models under various configurations, where 't' represents the temperature setting and 'n' denotes the number of examples per class used in few-shot prompting</em>

# Authors
[Jana Nikolovska](https://github.com/jananikolovska), [Marco Sangiorgi](https://github.com/SangioAI), [Andrea Fossà](https://github.com/andrea-fs)
