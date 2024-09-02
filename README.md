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
 
 Hasil dan Analisis

Model RNN yang dibangun mencapai akurasi di atas 98% pada data pelatihan, menunjukkan bahwa model mampu belajar dengan baik dari data. Namun, terdapat indikasi overfitting pada data validasi, yang ditunjukkan oleh peningkatan validation loss setelah beberapa epoch. Meski begitu, model tetap menunjukkan kemampuan yang baik dalam mengklasifikasikan pesan teks sebagai spam atau ham.
Kesimpulan

Proyek ini berhasil mengembangkan model yang efektif untuk klasifikasi teks menggunakan teknik RNN berbasis LSTM. Namun, untuk meningkatkan performa model lebih lanjut, disarankan untuk melakukan langkah-langkah seperti meningkatkan regularisasi, menambah data pelatihan, atau mencoba arsitektur model yang lebih kompleks.

Teknologi yang Digunakan

    Python: Digunakan untuk pengolahan data dan pengembangan model.
    Keras & TensorFlow: Framework yang digunakan untuk membangun dan melatih model neural network.
    Scikit-learn: Digunakan untuk preprocessing data dan evaluasi performa model.
    Numpy & Pandas: Untuk manipulasi data dan analisis numerik.
    Matplotlib & Seaborn: Untuk visualisasi data dan hasil evaluasi model.

GitHub Repository

Untuk melihat kode lengkap dari proyek ini, dokumentasi, dan instruksi tentang cara menjalankan proyek, kunjungi repository GitHub berikut: GitHub Repository.
