IDalam makalah ini, saya membahas sebuah metode untuk mengklasifikasikan pesan spam dengan menggunakan recurrent neural network (RNN).

Deskripsi Proyek

Proyek ini berpusat pada pembuatan model berdasarkan pembelajaran mesin yang memungkinkan identifikasi pesan sms sebagai spam atau ham. Dengan menggunakan Recurrent Neural Network (RNN) dengan Long Short-Term Memory (LSTM), model ini akan dapat mengidentifikasi pola dalam teks yang membedakan antara pesan spam dan pesan normal. Dataset

Data yang digunakan dalam proyek ini adalah SMS Spam Collection dan terdiri dari ribuan pesan teks yang diklasifikasikan sebagai spam atau ham. Dataset ini dimasukkan dari file CSV untuk pelatihan dan pengujian model di atas. Langkah-langkah Proyek

Data Preprocessing:

    Tokenisasi: Pra-pemrosesan teks: mengubah pesan teks menjadi token atau kata tunggal.
    Penghapusan Kata Henti: Penghapusan kata-kata berhenti yang tidak berguna dalam klasifikasi dokumen.
    Stemming: Membuat kata-kata sesederhana mungkin untuk mengurangi kompleksitas model dan mendapatkan hasil terbaik.
    Padding: Menormalkan pesan spam ke panjang yang diinginkan agar model LSTM dapat memproses semua pesan dengan benar.

Membangun Model RNN:

    Menerapkan lapisan LSTM untuk menangani urutan antar kata dalam teks.
    Menerapkan lebih banyak lapisan Dropout dan L2 Regularisation untuk menghindari overfitting.
    Untuk klasifikasi biner, digunakan lapisan padat dengan fungsi aktivasi sigmoid.

Pelatihan Model: Model yang diusulkan dilatih menggunakan pengoptimal Adam dan fungsi kehilangan entropi silang biner. Ada juga yang disebut Early Stopping yang digunakan untuk menghindari pelatihan yang berlebihan dan ini melibatkan penghentian proses pelatihan jika kinerja pada data validasi berkurang. Jenis mekanisme kontrol laju pembelajaran yang umum digunakan adalah Penjadwal Laju Pembelajaran yang membantu mengubah laju pembelajaran dalam proses pelatihan.

Evaluasi Model: Oleh karena itu, evaluasi dilakukan pada data uji untuk menentukan tingkat akurasi dan kerugian. Kerugian pelatihan dan validasi serta akurasi pelatihan dan validasi divisualisasikan untuk mengevaluasi kinerja model yang berbeda.
 
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
