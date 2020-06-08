# OCNN_SWAE
This is done as a part of my Analytics IV module. This is based on the papers [ANOMALY DETECTION USING ONE-CLASS NEURAL
NETWORKS](https://arxiv.org/pdf/1802.06360.pdf) and [Sliced-Wasserstein Autoencoder: An
Embarrassingly Simple Generative Model](https://arxiv.org/pdf/1804.01947.pdf). 

Though I am getting a good accuracy purely on the basis of Autoencoder alone, a lot more needs to be done in order to improve the accuracy of OCNN. 

The datasets chosen were the concrete crack datasets downloaded from [here](https://data.mendeley.com/datasets/5y9wdsg2zt/2)

1) Positive data extraction is documented [here](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/positive.ipynb) while the negative data extraction is documented [here](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/negative.ipynb)

2) Separate folders were created for the [positively](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/Creating%20Positive%20Data.ipynb) and negatively labelled [samples](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/Creating%20Negative%20Data.ipynb)

3) The data were resized and normalized based on the model requirements as documented [here](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/data_28_preprocessing.ipynb) and [here](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/data_64_preprocessing.ipynb)

4) 6 different models were trained and were named as [Model I](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/Training_Model1.ipynb), [Model II](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/Training_Model2.ipynb), [Model III](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/Training_Model3.ipynb), [Model IV](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/Training_Model4.ipynb), [Modev V](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/Training_Model5.ipynb) and [Model VI](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/Training_Model6.ipynb)

5) The validation data were [encoded and decoded](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/Encoding%20and%20Decoding%20Unseen%20Data.ipynb) for evaluation purposes

6) These models were [compared and evaluated](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/Autoencoder_Comparison.ipynb) using MSE, AUROC, Precision, Recall, Confusion Matrix, Accuracy Score and Classification Report

7) The encoded features of the best performing model across both balanced and biased datasets were chosen for further classification tasks using [OCNN](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/OCNN.ipynb)

The best performing model was Model VI which had an AUROC of 0.9909 on the balanced dataset and 0.9917 on the biased data.

All the raw data, processed data and pre-trained models can be found [here](https://drive.google.com/drive/u/0/folders/11IiIT5PLZK0ag01S6ZCZmCC_9E-PTHL1).
