# OCNN_SWAE
This is done as a part of my Analytics IV module. This is based on the papers [ANOMALY DETECTION USING ONE-CLASS NEURAL
NETWORKS](https://arxiv.org/pdf/1802.06360.pdf) and [Sliced-Wasserstein Autoencoder: An
Embarrassingly Simple Generative Model](https://arxiv.org/pdf/1804.01947.pdf). 

Though I am getting a good accuracy purely on the basis of Autoencoder alone, a lot more needs to be done in order to improve the accuracy of OCNN. 

Autoencoder training was based on the implementations [here](https://github.com/skolouri/swae) and OCNN was based on the implementations [here](https://github.com/danielenricocahall/One-Class-NeuralNetwork)

The datasets chosen were the concrete crack datasets downloaded from [here](https://data.mendeley.com/datasets/5y9wdsg2zt/2)

1) Positive data extraction is documented [here](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/positive%20(1).ipynb) while the negative data extraction is documented [here](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/negative%20(1).ipynb)

2) Separate folders were created for the [positively](hhttps://github.com/sidvenkat1988/OCNN_SWAE/blob/master/Creating%20Positive%20Data%20(1).ipynb) and negatively labelled [samples](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/Creating%20Negative%20Data%20(1).ipynb)

3) The data were resized and normalized based on the model requirements as documented [here](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/data_28_preprocessing%20(1).ipynb) and [here](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/data_64_preprocessing%20(1).ipynb)

4) 8 different models were trained and were named as [Model I](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/Training_Model1%20(1).ipynb), [Model II](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/Training_Model2%20(1).ipynb), [Model III](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/Training_Model3%20(1).ipynb), [Model IV](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/Training_Model4%20(1).ipynb), [Modev V](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/Training_Model5%20(1).ipynb), [Model VI](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/Training_Model6%20(1).ipynb), [Model VII](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/Training_Model7.ipynb) and [Model VIII](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/Training_Model8.ipynb)

5) The validation data were [encoded and decoded](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/Encoding%20and%20Decoding%20Unseen%20Data%20(1).ipynb) for evaluation purposes

6) These models were [compared and evaluated](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/Autoencoder_Comparison%20(1).ipynb) using MSE, AUROC, Precision, Recall, Confusion Matrix, Accuracy Score and Classification Report

7) The encoded features of the best performing model([Model VII](https://drive.google.com/drive/folders/1J-QYorfjpG2eXZKQu3iTVNToyKoiqfm8?usp=sharing)) across both balanced and biased datasets were chosen for further classification tasks using OCNN

8) 2 OCNN Models were trained and evaluated on balanced and imbalanced data, 1 with original features retained from the pre-trained Autoencoder model(documented [here](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/OCNN_Model_1.ipynb)) and 1 with pre-trained features halved by PCA(documented [here](https://github.com/sidvenkat1988/OCNN_SWAE/blob/master/OCNN_MODEL_2.ipynb))

All the raw data, processed data and pre-trained models can be found [here](https://drive.google.com/drive/u/0/folders/11IiIT5PLZK0ag01S6ZCZmCC_9E-PTHL1).
