# Deep-Learning-Final-Project
The project is implementation of two different research papers and comparing their performance to each other as well as to the original paper.

## Research papers used
1. A Dual-Stage Attention-Based Recurrent Neural Network for Time Series Prediction
https://arxiv.org/abs/1704.02971

2. Hierarchical Attention-Based Recurrent Highway Networks for Time Series Prediction
https://arxiv.org/abs/1806.00685

## Dataset
Here we have used a timeseries dataset of NASDAQ stock data of 105 trading days from 26th July,2016 to December 22,2016

## Model 1:
 ![alt text](https://github.com/sharan165/Deep-Learning-Project/blob/main/images/DARNN_model.PNG 'DA-RNN')
 
The paper here proposes a novel method of capturing both the long term dependancies as well as important hidden variables from the input data.

The neural network here consists of two parts: input attention mechanism and temporal attention mechanism. 

•	In input attention mechanism the network layers try to capture only the most important hidden variables at each time step before feeding that data into the encoder LSTM network. 

•	In temporal attention mechanism the relevant encoder hidden states that are extracted across all time steps are retrieved from the LSTM encoder and integrated with the hidden state of the LSTM decoder. The network layers then try to capture the important hidden variables from the encoder and decoder combined. 

## Model 2:
![alt text](https://github.com/sharan165/Deep-Learning-Project/blob/main/images/HARHN_model.PNG "HA-RNN")

•	The encoder here consists of convolution layer blocks or a network of convolution networks along with Recurrent Highway network.

•	This part of the network is used to model the exogenous temporal dynamics of the input.

•	Most important use of CNN here is its ability to learn the feature representation by convolving the inputs and summarizing them.

•	The Recurrent Highway networks is the part use to model the temporal dynamics of the exogenous series of inputs.

•	The decoder here also consists of a RHN which not only helps to decode the temporal dynamics of the old data but also the correlations among the data used to train.


## Libraries/Tools Used
1. Pandas
2. Numpy
3. Pytorch
4. Matplotlib
5. Jupyter Notebook

## Results achieved
Here we are getting results close to the original paper but still needs some work to replicate exact same results as the researcch paper

## Running the notebook
Use the dataset given in the repository and follow the along the notebook.


