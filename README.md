# Movie Recommendation System

## Deskripsi Proyek

Proyek ini merupakan sistem rekomendasi film sederhana yang memanfaatkan data film dan rating pengguna untuk memberikan rekomendasi film berdasarkan judul film yang dicari. Sistem ini menggunakan metode pengolahan teks TF-IDF untuk pencarian film berdasarkan kemiripan judul, dan analisis rating pengguna untuk merekomendasikan film-film yang disukai oleh pengguna lain yang juga menyukai film tersebut.

---

## Fitur

* **Pencarian Film**
  Pengguna dapat memasukkan judul film, dan sistem akan mencari film dengan judul paling mirip menggunakan TF-IDF dan cosine similarity.

* **Rekomendasi Film**
  Berdasarkan film yang dicari, sistem memberikan rekomendasi film yang disukai oleh pengguna lain yang juga menyukai film tersebut, dengan mempertimbangkan popularitas dan kesamaan preferensi.

* **Antarmuka Interaktif**
  Menggunakan `ipywidgets` untuk membuat input pencarian film dan menampilkan hasil rekomendasi secara interaktif di Jupyter Notebook.

---

## Dataset

* **movies.csv**: Data daftar film dengan kolom `movieId`, `title`, dan `genres`.
* **ratings.csv**: Data rating pengguna terhadap film, dengan kolom `userId`, `movieId`, `rating`, dan `timestamp`.

---

## Cara Menjalankan

1. Clone repository ini:

   ```bash
   git clone https://github.com/username/movie-recommendation.git
   cd movie-recommendation
   ```

2. Pastikan kamu sudah menginstall library yang dibutuhkan:

   ```bash
   pip install pandas scikit-learn ipywidgets
   ```

3. Siapkan dataset `movies.csv` dan `ratings.csv` di folder project (bisa didownload dari MovieLens).

4. Buka Jupyter Notebook dan jalankan file notebook atau script Python yang ada.

5. Masukkan judul film pada widget input, dan tunggu rekomendasi film muncul secara interaktif.

---

## Struktur Proyek

```
movie-recommendation/
│
├── movies.csv
├── ratings.csv
├── recommendation.ipynb   # Notebook utama berisi kode sistem rekomendasi
├── README.md
```

---

## Penjelasan Kode (Ringkas)

* **Data Loading & Preprocessing**
  Membaca data film dan rating, membersihkan judul film untuk memudahkan pencarian.

* **TF-IDF Vectorization**
  Mengubah judul film menjadi vektor untuk pencarian kemiripan teks.

* **Fungsi Pencarian**
  Mencari film berdasarkan kemiripan judul menggunakan cosine similarity.

* **Fungsi Rekomendasi**
  Menghitung film yang paling sering disukai oleh pengguna yang juga menyukai film yang dicari.

* **Antarmuka Interaktif**
  Membuat widget input dan output rekomendasi yang responsif di notebook.

---
