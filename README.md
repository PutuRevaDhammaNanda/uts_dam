# UTS Data Acquisition & Management
## Akuisisi dan Integrasi Data Pariwisata Indonesia

### Identitas
- **Nama:** Putu Reva Dhamma Nanda
- **NIM:** 2501010167
- **Mata Kuliah:** Data Acquisition & Management
- **Kelas:** F

---

## 1. Deskripsi Proyek

Proyek ini membahas proses akuisisi dan integrasi data pariwisata Indonesia dari beberapa sumber. Data diperoleh melalui dataset CSV, API, dan web scraping. Data yang dikumpulkan mencakup informasi destinasi wisata, data cuaca, dan data populasi kota.

## 2. Tujuan Proyek

- Mengumpulkan data pariwisata dari berbagai sumber.
- Mengidentifikasi karakteristik dan kualitas dataset.
- Memeriksa lisensi serta etika penggunaan data.
- Melakukan akuisisi data melalui API dan web scraping.
- Melakukan cleaning dan normalisasi data.
- Mengintegrasikan data dari beberapa sumber.
- Menghasilkan dataset pariwisata terintegrasi.

## 3. Sumber Data

### Sumber 1 Dataset Pariwisata Indonesia
- **Sumber:** Kaggle
- **Nama Dataset:** Indonesia Tourism Destination
- **Metode Akuisisi:** Download dataset CSV
- **URL:** https://www.kaggle.com/datasets/aprabowo/indonesia-tourism-destination
- **Data:** Nama destinasi, kota, kategori, koordinat, harga, rating, dan informasi lainnya.

### Sumber 2  API Cuaca
- **Sumber:** Open-Meteo
- **Metode Akuisisi:** HTTP Request menggunakan Python Requests
- **URL:** https://api.open-meteo.com/v1/forecast
- **Dokumentasi:** https://open-meteo.com/en/docs
- **Data:** Temperatur, kelembapan, curah hujan, kecepatan angin, waktu pengukuran, dan timezone.
- **Jumlah Data:** 30 destinasi wisata.

### Sumber 3  Data Populasi Kota
- **Sumber:** Wikipedia
- **Metode Akuisisi:** Web Scraping menggunakan Python Requests dan Pandas `read_html`
- **URL:** https://en.wikipedia.org/wiki/List_of_Indonesian_cities_by_population
- **Data:** Informasi populasi kota yang dicocokkan dengan dataset pariwisata.

## 4. Metode Pengolahan dan Integrasi

Tahapan pengerjaan proyek:

1. Mengunduh dataset pariwisata Indonesia.
2. Membaca dan mengidentifikasi karakteristik dataset.
3. Memeriksa lisensi dan etika penggunaan data.
4. Mengambil data cuaca melalui API Open-Meteo.
5. Memeriksa `robots.txt` sebelum melakukan scraping.
6. Mengambil halaman HTML dan mengekstrak tabel populasi kota.
7. Melakukan cleaning dan normalisasi data.
8. Mengintegrasikan dataset pariwisata dengan data cuaca.
9. Mengintegrasikan data populasi kota.
10. Melakukan validasi hasil integrasi.

## 5. Hasil Proyek

Hasil akhir proyek berupa dataset pariwisata Indonesia yang telah diintegrasikan dengan data cuaca dan populasi kota.

Dataset hasil integrasi disimpan dalam file:

`data/processed/tourism_integrated.csv`

Hasil lainnya meliputi data mentah, data hasil normalisasi, JSON tabular, HTML tabular, dokumentasi provenance, dan Data Ethics Checklist.

