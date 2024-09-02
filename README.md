In this paper, I discuss a method of classifying spam messages using the recurrent neural network (RNN). 
 
 Project Description 
 
 This project is centered on creating a model based on machine learning that will enable the identification of sms messages as either spam or ham. From using Recurrent Neural Network (RNN) with Long Short-Term Memory (LSTM), the model will be able to identify patterns in the text that discriminates between the spam messages and normal messages. 
 Dataset 
 
 The data used in this project is the SMS Spam Collection and it consist of thousands of text messages which are classified as spam or ham. It entered this dataset from a CSV file for training and testing the above model. 
 Project Steps 
 
 Data Preprocessing: 
 - Tokenisation: Text pre-processing: converting text messages to tokens or single words. 
 - Stopwords Removal: Elimination of the stop words which are not useful in the classification of the documents. 
 - Stemming: Make words as simple as possible so as to reduce model complexity and to get the best results. 
 - Padding: Normalises spam messages to the intended length to allow LSTM model to process all of the messages properly. 
 
 Building the RNN Model: 
 - Applying LSTM layer for handling with the order between words in text. 
 - Implemented more Dropout and L2 Regularisation layers for the purpose of avoiding overfitting. 
 - For binary classification Dense layer with sigmoid activation function is used. 
 
 Model Training: 
 The proposed model was trained using Adam optimiser and binary cross entropy loss function. 
 Another was called Early Stopping which was used to avoid over-training and this involved stopping the training process if the performance on the validation data reduced. 
 A common type of learning rate control mechanism is Learning Rate Scheduler which helps to change the learning rate in the process of training. 
 
 Model Evaluation: 
 Therefore, evaluation is conducted on the test data to determine the level of accuracy and loss. 
 Training and validation loss as well as training and validation accuracy were visualized to evaluate the different performance of the model. 
 
 
