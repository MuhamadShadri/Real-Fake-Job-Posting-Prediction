# Submission 1: Real / Fake Job Posting Prediction

Nama: Muhamad Shadri

Username Dicoding: [muhamad_shadri](https://www.dicoding.com/users/muhamad_shadri/academies)

|     | Deskripsi |
| --- | --------- |
| Dataset | [Real / Fake Job Posting Prediction](https://www.kaggle.com/datasets/shivamb/real-or-fake-fake-jobposting-prediction) |
| Latar Belakang | Pencarian kerja melalui platform online telah menjadi salah satu metode utama bagi banyak orang untuk mencari pekerjaan. Namun, seiring dengan meningkatnya jumlah lowongan pekerjaan yang diposting secara daring, jumlah iklan pekerjaan palsu juga meningkat. Iklan pekerjaan palsu ini dapat menipu pencari kerja, menyebabkan kerugian finansial, dan membuang-buang waktu yang berharga. Oleh karena itu, sangat penting untuk memiliki kemampuan untuk mengidentifikasi apakah suatu iklan pekerjaan itu asli atau palsu. |
| Masalah | Jumlah posting pekerjaan palsu yang meningkat membuat sulit bagi pencari kerja untuk membedakan antara posting pekerjaan yang asli dan yang palsu. Tanpa alat yang tepat, pencari kerja dapat dengan mudah tertipu oleh posting pekerjaan palsu. Ini tidak hanya mengakibatkan kerugian finansial tetapi juga dapat menyebabkan kerugian emosional dan waktu yang signifikan. |
| Solusi Machine Learning | Untuk mengatasi masalah ini, diperlukan sistem yang dapat mengklasifikasikan posting pekerjaan apakah asli atau palsu. Dengan menggunakan teknik machine learning, sistem ini dapat membantu menyaring posting pekerjaan yang relevan dan mengidentifikasi posting pekerjaan yang mencurigakan. Ini akan membantu pencari kerja untuk fokus pada lowongan pekerjaan yang sah dan menghindari penipuan. |
| Metode Pengolahan Data | Proses pengolahan data dalam proyek ini dimulai dengan menghilangkan atau menghapus beberapa atribut yang tidak relevan, lalu dilanjutkan dengan langkah pengambilan data (Data Ingestion) yang membagi dataset menjadi data training dan evaluasi dengan perbandingan 9:1. Langkah berikutnya adalah validasi data (Data Validation) yang melibatkan pemeriksaan statistik, skema data, serta deteksi anomali dalam dataset. Selanjutnya, dilakukan tahapan pra-pemrosesan data (Data Preprocessing) dengan melakukan transformasi fitur pada input data. Dengan demikian, data siap untuk digunakan dalam proses analisis lebih lanjut. |
| Arsitektur Model | Struktur model yang dirancang terdiri dari serangkaian lapisan untuk mengolah data teks. Pertama, terdapat lapisan masukan (input layer) yang menerima teks atau string sebagai input, yang kemudian diproses oleh lapisan TextVectorization untuk mengonversi teks menjadi representasi numerik. Selanjutnya, terdapat lapisan Embedding dan Bidirectional LSTM untuk mempelajari pola dan hubungan antar kata dalam teks. Selain itu, model memiliki dua lapisan tersembunyi (hidden layer) yang terdiri dari Dense layer, diikuti oleh satu lapisan keluaran (output layer). Dengan struktur ini, model mampu memahami dan menginterpretasikan informasi dari teks dengan lebih baik untuk tujuan klasifikasi. |
| Metrik Evaluasi | Pada evaluasi performa model machine learning, sejumlah metrik digunakan untuk mengukur kinerja. Antara lain, metrik AUC (Area Under the ROC Curve) yang mengukur seberapa baik model memisahkan kelas positif dan negatif, serta Binary Accuracy yang menentukan seberapa akurat model dalam memprediksi kelas. Selain itu, metrik lainnya seperti TFMA Example Count, False Negatives, False Positives, True Negatives, dan True Positives juga digunakan untuk memberikan wawasan lebih mendalam tentang bagaimana model menangani setiap kelas dan jenis kesalahan yang terjadi. Dengan berbagai metrik ini, evaluasi model menjadi lebih komprehensif dan dapat memberikan informasi yang lebih detail tentang kinerja model dalam konteks spesifik. |
| Performa Model | Kinerja model yang telah dikembangkan dinilai cukup baik dan optimal dengan tingkat `binary_accuracy` sebesar 97% dan `val_binary_accuracy` sebesar 98%. |
| Kesimpulan | Dengan membangun model ini, diharapkan dapat memberikan pemahaman yang lebih baik tentang apakah suatu postingan pekerjaan online asli atau palsu. Hal ini menjadi penting dalam melindungi pencari kerja dari penipuan dan kerugian finansial yang mungkin timbul akibat menerima tawaran pekerjaan palsu. Dengan menggunakan teknik machine learning untuk mengklasifikasikan postingan pekerjaan, model ini dapat menjadi alat yang berguna dalam memitigasi risiko penipuan dalam pasar kerja online dan memberikan perlindungan kepada masyarakat yang mencari pekerjaan secara daring. |
