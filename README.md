# ☕ Clustering Potensi Kopi (Web GIS)

Aplikasi ini adalah implementasi sistem **Geographic Information System (GIS)** untuk mengelompokkan (clustering) daerah potensi penghasil kopi menggunakan algoritma **K-Means**.

Proyek ini disusun sebagai bagian dari Tugas Akhir / Skripsi di **Universitas Sulawesi Barat**.

## 👤 Identitas Pengembang
* **Nama:** Abdullah Azzam
* **NIM:** D0221304
* **Jurusan:** Teknik Informatika

## 📖 Deskripsi Singkat
Sistem ini bertujuan untuk memetakan dan mengelompokkan wilayah berdasarkan potensi produktivitas kopi. Dengan menggunakan metode **K-Means Clustering**, daerah dikelompokkan menjadi beberapa klaster (misal: Potensi Tinggi, Sedang, Rendah) untuk membantu pengambilan keputusan strategis.

## 🌟 Fitur Utama
* **Visualisasi Peta:** Menampilkan sebaran lokasi lahan kopi menggunakan peta interaktif (LeafletJS / Google Maps).
* **Algoritma K-Means:** Perhitungan otomatis untuk mengelompokkan data berdasarkan atribut (luas lahan, hasil panen, ketinggian, dll).
* **Manajemen Data:** CRUD (Create, Read, Update, Delete) data lokasi dan hasil panen.
* **Laporan:** Ekspor hasil clustering.

## 🛠️ Teknologi yang Digunakan
* **Bahasa Pemrograman:** (PHP Native / Laravel / Python Flask) - *Sesuaikan dengan isi kodinganmu*
* **Database:** MySQL
* **Frontend:** HTML, CSS, Bootstrap
* **Peta:** Leaflet.js / Mapbox / Google Maps API

## 📂 Struktur Folder
* `/assets` - File CSS, JS, dan gambar.
* `/config` - Konfigurasi koneksi database.
* `/modules` - Logika perhitungan K-Means.
* `index.php` - Halaman utama dashboard.

## 🚀 Cara Menjalankan (Localhost)

1.  **Clone Repositori:**
    ```bash
    git clone [https://github.com/Zaammm16/Cluster.git](https://github.com/Zaammm16/Cluster.git)
    ```
2.  **Import Database:**
    * Buat database baru di phpMyAdmin bernama `db_clustering`.
    * Import file `.sql` yang ada di folder `database` (jika ada).
3.  **Konfigurasi Koneksi:**
    * Sesuaikan file `koneksi.php` atau `.env` dengan username/password database lokal Anda.
4.  **Jalankan di Browser:**
    * Buka `http://localhost/Cluster`

## 📊 Metode K-Means
Aplikasi ini menggunakan alur perhitungan K-Means standar:
1.  Penentuan jumlah klaster (K).
2.  Inisialisasi centroid secara acak.
3.  Perhitungan jarak data ke centroid (Euclidean Distance).
4.  Pengelompokan data berdasarkan jarak terdekat.
5.  Iterasi hingga posisi centroid konvergen (tidak berubah).

---
*Dibuat oleh Abdullah Azzam (2025).*
