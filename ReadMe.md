# README

## Proyek: Rekomendasi Kebijakan Publik untuk Jakarta Timur

### Deskripsi

Proyek ini bertujuan untuk memberikan rekomendasi kebijakan publik berdasarkan data jumlah penduduk lanjut usia di setiap kelurahan di Jakarta Timur. Data yang digunakan bersumber dari dataset mengenai jumlah penduduk lanjut usia berdasarkan jenis kelamin, usia, dan lokasi per kelurahan.

### Fitur Utama

1. **Preprocessing Data:**

   - Menghapus data dari tahun 2015 hingga 2017.
   - Memfilter data khusus untuk wilayah Jakarta Timur.

2. **Analisis Kuantitatif:**

   - Mengelompokkan data jumlah penduduk lanjut usia per kelurahan.
   - Menentukan ambang batas (kuartil ke-75 dan ke-25) untuk memberikan rekomendasi.

3. **Rekomendasi Kebijakan Publik:**

   - **Tambah Fasilitas Kesehatan** untuk kelurahan dengan jumlah penduduk lanjut usia di atas kuartil ke-75.
   - **Tingkatkan Kegiatan Sosial** untuk kelurahan dengan jumlah penduduk lanjut usia di bawah kuartil ke-25.
   - **Pantau dan Evaluasi** untuk kelurahan dengan jumlah penduduk lanjut usia di antara kedua ambang batas tersebut.

4. **Visualisasi Data:**

   - Membuat visualisasi berupa diagram batang yang menunjukkan rekomendasi kebijakan untuk setiap kelurahan.

5. **Ekspor Hasil:**
   - Hasil analisis dan rekomendasi disimpan dalam file CSV

### Struktur Proyek

- **Input Data:**
  - File CSV yang berisi data jumlah penduduk lanjut usia berdasarkan jenis kelamin, usia, dan lokasi per kelurahan.
- **Output Data:**
  - File CSV yang berisi kelurahan, jumlah penduduk lanjut usia, dan rekomendasi kebijakan.
- **Visualisasi:**
  - Diagram batang yang menunjukkan jumlah penduduk lanjut usia per kelurahan dan kebijakan yang direkomendasikan.

### Cara Menggunakan

1. **Persiapan Lingkungan:**

   - Pastikan Anda memiliki Python 3.x terinstal.
   - Instal pustaka yang diperlukan:
     ```bash
     pip install pandas numpy matplotlib scikit-learn
     ```

2. **Menjalankan Kode:**

   - Simpan dataset Anda dalam file CSV bernama `Filedata Data Jumlah Penduduk Lanjut Usia Berdasarkan Jenis Kelamin dan Usia Per Kelurahan.csv`.
   - Jalankan skrip Python:
     ```bash
     python rekomendasi_kebijakan.py
     ```

3. **Hasil:**
   - Hasil analisis akan dicetak di terminal.
   - File CSV hasil analisis akan disimpan dengan nama `Rekomendasi_Kebijakan_Jakarta_Timur.csv`.
   - Visualisasi akan ditampilkan dalam bentuk diagram batang.

### Contoh Hasil

**File CSV Output:**
| Kelurahan | Jumlah Penduduk | Rekomendasi Kebijakan |
|-------------------|-----------------|--------------------------------|
| Kelurahan A | 1200 | Tambah Fasilitas Kesehatan |
| Kelurahan B | 400 | Tingkatkan Kegiatan Sosial |
| Kelurahan C | 800 | Pantau dan Evaluasi |

**Visualisasi:**

- Diagram batang menunjukkan jumlah penduduk lanjut usia per kelurahan dengan warna yang merepresentasikan kategori kebijakan.

### Catatan

- Dataset harus memiliki kolom `Nama_Kabupaten_Kota`, `Kelurahan`, `Jumlah Penduduk`, dan `Tahun` agar skrip dapat berjalan dengan benar.
- Parameter ambang batas dapat disesuaikan jika diperlukan.

Dikembangkan oleh: [Fakhri Andika]
Link PPT : [Klik disini](https://www.canva.com/design/DAGbnsmKQnE/jXaG_ayoPpzaOSdiMJrwZQ/edit)
