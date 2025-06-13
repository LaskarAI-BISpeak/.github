# [LAI25-SM055] Laskar AI BiSpeak Project  BISINDO

✨ *Bagian dari Laskar AI Cohort 2025* ✨

Selamat datang di repositori Proyek BiSpeak! Kami adalah tim Laskar AI SM055 yang  mengembangkan sebuah **Image Classifier untuk Bahasa Isyarat Indonesia (BISINDO)**.

---

## 👨‍👩‍👧‍👦 Tim Kami (Our Team)

Kami adalah kelompok kami:

| ID         | Nama                | Universitas                          | Email                       | GitHub                                   |
| :--------- | :------------------ | :----------------------------------- | :-------------------------- | :--------------------------------------- |
| A548YBM523 | Zulfahmi M. Ardianto | UIN Sunan Kalijaga                   | A548YBM523@dicodingacademy.id | [7z1x](https://github.com/7z1x)          |
| A013XBM217 | Idha Kurniawati     | Universitas Terbuka                  | A013XBM217@dicodingacademy.id | [idhak](https://github.com/idhak)       |
| A203XBM381 | Nurfadilah          | Universitas Duta Bangsa Surakarta    | A203XBM381@dicodingacademy.id | [smithdilah](https://github.com/smithdilah)|
| A228XBM423 | Ria Kristi          | Universitas Jenderal Achmad Yani Yogyakarta | A228XBM423@dicodingacademy.id | [riakrst](https://github.com/riakrst)   |

---

## 📌 Gambaran Umum Proyek (Project Overview)

BiSpeak adalah proyek inovatif yang bertujuan untuk menjembatani kesenjangan komunikasi bagi komunitas Tuli melalui pengembangan model klasifikasi gambar Bahasa Isyarat Indonesia (BISINDO) berbasis *machine learning*. Model kami dirancang untuk dapat mendeteksi dan menginterpretasikan gestur tangan dari sebuah gambar, kemudian mengklasifikasikannya ke dalam kategori huruf maupun kata-kata spesifik dalam BISINDO.

Dengan sistem klasifikasi gambar BISINDO yang akurat, kami berharap proyek ini dapat menjadi landasan bagi pengembangan aplikasi penerjemah bahasa isyarat secara *real-time*. Hal ini diharapkan dapat mendukung komunikasi yang lebih efektif dan inklusif, baik antar pengguna BISINDO maupun antara pengguna BISINDO dengan masyarakat umum.

---

## 🚀 Fitur Utama (Features)

Berikut adalah beberapa fitur yang kami rencanakan untuk dikembangkan dalam proyek BiSpeak:

* ✅ **Klasifikasi Alfabet BISINDO**: Kemampuan untuk mengenali dan membedakan setiap huruf dalam sistem alfabet BISINDO.
* ✅ **Klasifikasi Kata Umum BISINDO**: Pengembangan untuk mengenali beberapa kata atau frasa umum yang sering digunakan dalam BISINDO.
* 📊 **Visualisasi Hasil Prediksi**: Menampilkan hasil klasifikasi dengan jelas beserta tingkat kepercayaan (confidence score).
* 🧩 **Antarmuka Pengguna Sederhana**: (Opsional) Jika dikembangkan menjadi aplikasi, akan memiliki antarmuka yang mudah digunakan.

*(Fitur-fitur ini akan diperbarui seiring dengan progres pengembangan)*

---

## 🧠 Model & Dataset

Detail mengenai arsitektur model dan dataset yang kami gunakan akan dijabarkan di sini.

* **Model yang Digunakan**:
    * Eksperimen awal dilakukan dengan arsitektur seperti **MobileNetV2** dan **EfficientNet** karena efisiensinya untuk aplikasi *mobile* atau *real-time*.
    * Teknik *transfer learning* juga dipertimbangkan untuk meningkatkan akurasi dengan data yang terbatas.
* **Dataset**:
    * **Jumlah Kelas**: [Contoh: 26 kelas untuk alfabet, X kelas untuk kata].
    * **Ukuran Dataset**: [Contoh: Sekitar N gambar per kelas, total M gambar].
    * **Pra-pemrosesan**: Langkah-langkah seperti augmentasi data (rotasi, flip, zoom), normalisasi, dan segmentasi tangan untuk meningkatkan kualitas input model.

*(Informasi lebih detail akan ditambahkan setelah proses eksperimen dan evaluasi model selesai)*

---

---
## 🗂️ Struktur Folder Proyek

```
LaskarAI-BISpeak/
│
├── BISINDO-Image-Classification-Model/
│   └── app.py
│   └── collect_images.py
│   └── create_dataset_1_hand.py
│   └── create_dataset_2_hand.py
|   └── data_1_tangan.pickle
|   └── data_2_tangan.pickle
|   └── inference.py
|   └── model_1_hand.p
|   └── model_2_hand.p
|   └── packages.txt
|   └── requirements.txt
|   └── train_classifier.py
│
├── dataset/
│   └── dataset_1_tangan
│   └── dataset_2_tangan
│
└── README.md
```

---
