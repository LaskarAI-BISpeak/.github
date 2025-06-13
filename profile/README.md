# 🧐 [LAI25-SM055] Proyek BiSpeak – BISINDO Image Classifier

✨ *Bagian dari Program Laskar AI Cohort 2025* ✨

Selamat datang di repositori **BiSpeak**, sebuah proyek inovatif dari tim **LAI25-SM055**. Kami mengembangkan sistem **klasifikasi citra untuk Bahasa Isyarat Indonesia (BISINDO)**, yang bertujuan mendukung komunikasi lebih inklusif bagi komunitas Tuli di Indonesia.

---

## 👥 Tim Kami

| ID         | Nama                 | Universitas                                 | Email                                                                  | GitHub                                      |
| ---------- | -------------------- | ------------------------------------------- | ---------------------------------------------------------------------- | ------------------------------------------- |
| A548YBM523 | Zulfahmi M. Ardianto | UIN Sunan Kalijaga                          | [A548YBM523@dicodingacademy.id](mailto\:A548YBM523@dicodingacademy.id) | [7z1x](https://github.com/7z1x)             |
| A013XBM217 | Idha Kurniawati      | Universitas Terbuka                         | [A013XBM217@dicodingacademy.id](mailto\:A013XBM217@dicodingacademy.id) | [idhak](https://github.com/idhak)           |
| A203XBM381 | Nurfadilah           | Universitas Duta Bangsa Surakarta           | [A203XBM381@dicodingacademy.id](mailto\:A203XBM381@dicodingacademy.id) | [smithdilah](https://github.com/smithdilah) |
| A228XBM423 | Ria Kristi           | Universitas Jenderal Achmad Yani Yogyakarta | [A228XBM423@dicodingacademy.id](mailto\:A228XBM423@dicodingacademy.id) | [riakrst](https://github.com/riakrst)       |

---

## 📌 Gambaran Umum Proyek

**BiSpeak (BISINDO Speak)** adalah sistem klasifikasi citra yang dapat mengenali posisitangan dalam Bahasa Isyarat Indonesia (BISINDO) secara real-time. Proyek ini dibangun dengan memanfaatkan **MediaPipe** untuk mengekstraksi fitur landmark tangan, dan **algoritma Random Forest** untuk mengklasifikasikan hasil ke dalam huruf dan kata BISINDO.

Dengan pendekatan ini, BiSpeak diharapkan menjadi langkah awal dalam pengembangan alat bantu komunikasi berbasis AI untuk mendukung interaksi antara Teman Tuli dan masyarakat luas. Sistem ini juga diimplementasikan dalam antarmuka berbasis **Streamlit**, sehingga memungkinkan pengujian dan penggunaan langsung oleh pengguna.

---

## 🚀 Fitur Unggulan

👉 **Klasifikasi Huruf BISINDO**: Mampu mengenali alfabet A–Z berdasarkan gesture tangan.\
👉 **Klasifikasi Kata Umum BISINDO**: Mendeteksi isyarat kata-kata umum dalam percakapan sehari-hari.\
📊 **Visualisasi Hasil Prediksi**: Menampilkan label hasil klasifikasi serta tingkat akurasinya.\
💻 **Antarmuka Streamlit Interaktif**: Memungkinkan pengguna untuk melakukan inferensi secara real-time dengan gambar atau webcam.

---

## 🧠 Model & Dataset

### 🔍 Model

- **Ekstraksi Fitur**: Menggunakan **MediaPipe Hands** untuk mendapatkan 21 titik koordinat tangan.
- **Algoritma Klasifikasi**: Menggunakan **Random Forest** untuk efisiensi dan kecepatan dalam inferensi.
- **Eksperimen Awal**: Juga dilakukan dengan transfer learning menggunakan arsitektur seperti MobileNetV2 dan EfficientNet.

### 📂 Dataset

- **Jumlah Data**: \~23.000 gambar gesture tangan
- **Jumlah Kelas**:
  - 26 kelas untuk huruf (A–Z)
  - 20 kelas untuk kata (Ayah, Berjalan, Bermain, Bicara, Duduk, Kamu, Maaf, Makan, Membaca, Melihat,  
Minum, Saya, Siapa, Halo, Ibu, Suka, Terima Kasih, Nama, Rumah, Sehat)
- **Metode Pengumpulan**: Pengambilan gambar mandiri oleh tim menggunakan skrip otomatis.
---

## 🗂️ Struktur Folder Proyek

```
LaskarAI-BISpeak/
│
├── BISINDO-Image-Classification-Model/
│   ├── app.py                      # Aplikasi Streamlit
│   ├── collect_images.py          # Skrip pengambilan data
│   ├── create_dataset_1_hand.py   # Dataset 1 tangan
│   ├── create_dataset_2_hand.py   # Dataset 2 tangan
│   ├── inference.py               # Modul inferensi
│   ├── model_1_hand.p
│   ├── model_2_hand.p
│   ├── packages.txt
│   ├── requirements.txt
│   └── train_classifier.py        # Skrip pelatihan model
│
└── README.md
```

---

## 📣 Catatan

Proyek ini masih dalam tahap pengembangan. Beberapa fitur dan arsitektur dapat berubah berdasarkan hasil evaluasi dan uji coba lanjutan. Kami terbuka terhadap kontribusi dan masukan dari komunitas.

