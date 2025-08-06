# 🏢 JobStreet Company Intelligence Crawler

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Python](https://img.shields.io/badge/Python-3.9%2B-blue?logo=python)
![Selenium](https://img.shields.io/badge/Selenium-4-green?logo=selenium)

Tool crawling profesional untuk mengekstrak informasi detail perusahaan dari JobStreet Indonesia secara otomatis. Dibuat untuk tujuan penelitian dan analisis data perusahaan.

## ✨ Fitur Utama

- **🔍 Pencarian Multi-Keyword**: Mampu melakukan pencarian untuk beberapa perusahaan sekaligus dalam satu sesi.
- **📊 Data Komprehensif**: Mengekstrak nama, rating, ulasan, website, industri, ukuran, dan lokasi perusahaan.
- **🎨 Antarmuka Profesional**: Dilengkapi GUI berbasis IPython Widgets yang modern dan mudah digunakan.
- **💾 Ekspor Multi-Format**: Mendukung ekspor data hasil crawling ke format **Excel (.xlsx)**, **CSV**, dan **JSON**.
- **🚀 Otomasi Penuh**: Menggunakan Selenium WebDriver dengan Chrome headless untuk proses crawling yang stabil dan tidak mengganggu.
- **⚡ Auto-Install Dependensi**: Skrip akan secara otomatis menginstal pustaka yang dibutuhkan saat pertama kali dijalankan.

## 🔧 Tumpukan Teknologi (Tech Stack)

- **Automasi Browser**: `Selenium WebDriver`
- **Parsing HTML**: `BeautifulSoup4`
- **Manipulasi Data**: `Pandas`
- **Antarmuka Pengguna**: `IPython Widgets`
- **Manajemen Driver**: `webdriver-manager`
- **Permintaan HTTP**: `requests`

## 🚀 Cara Memulai

### Prasyarat
- Lingkungan Python (direkomendasikan Anaconda/Jupyter Notebook).
- Browser Google Chrome terinstal di sistem Anda.

### Instalasi
Proyek ini dirancang untuk kemudahan maksimal. Anda tidak perlu melakukan instalasi manual.
Cukup jalankan **Cell (Tahap 1)** di dalam notebook, dan semua pustaka yang diperlukan akan diinstal secara otomatis.

### Petunjuk Penggunaan

1.  **Jalankan Semua Tahapan**: Eksekusi semua cell dari atas ke bawah secara berurutan:
    - `✅ Tahap 1: Import & Setup Pustaka`
    - `✅ Tahap 2: Setup Driver & Fungsi Crawling`
    - `✅ Tahap 3: Event Handlers & Logika Pemrosesan`
    - `✅ Tahap 4: Interface Widget Profesional`

2.  **Masukkan Keywords**: Setelah antarmuka pengguna muncul, masukkan nama-nama perusahaan di dalam kotak teks yang tersedia.
    - **Untuk beberapa perusahaan**, pisahkan setiap nama dengan baris baru (Enter).
    - **Contoh Input**:
      ```
      Bank BCA
      Telkom Indonesia
      PT Astra International
      Gojek
      ```

3.  **Mulai Crawling**: Klik tombol **`🚀 Mulai Crawling`**. Proses akan berjalan di latar belakang (headless). Anda dapat memonitor status dan log kemajuan di area output.

4.  **Lihat & Ekspor Data**:
    - Setelah proses selesai (ditandai dengan status berwarna hijau), klik **`📊 Lihat Data`** untuk menampilkan hasil dalam format tabel.
    - Gunakan tombol ekspor (**`📄 Excel`**, **`📊 CSV`**, **`🔗 JSON`**) untuk menyimpan data ke dalam file.
    - Klik **`🗑️ Bersihkan`** untuk mereset data dan antarmuka sebelum memulai sesi baru.

## 📊 Struktur Data Output

Data yang berhasil diekstrak akan memiliki kolom-kolom berikut:

| Field           | Deskripsi                                    | Contoh                                     |
| --------------- | -------------------------------------------- | ------------------------------------------ |
| `search_keyword`| Kata kunci pencarian yang digunakan          | "Bank BCA"                                 |
| `company_name`  | Nama resmi perusahaan                        | "PT Bank Central Asia Tbk"                 |
| `rating`        | Rating perusahaan (skala 5)                  | "4.2"                                      |
| `reviews_count` | Jumlah ulasan dari karyawan                  | "1,234 reviews"                            |
| `website`       | URL website resmi perusahaan                 | "https://www.bca.co.id"                    |
| `industry`      | Sektor industri perusahaan                   | "Banking & Financial Services"             |
| `company_size`  | Ukuran perusahaan (jumlah karyawan)          | "10,000+ employees"                        |
| `location`      | Lokasi utama perusahaan                      | "Jakarta, Indonesia"                       |
| `final_url`     | URL halaman detail di JobStreet              | "https://id.jobstreet.com/companies/..."   |

## 💡 Tips & Troubleshooting

- **Error pada Chrome Driver**: Jika terjadi error, coba restart kernel notebook Anda dan jalankan kembali semua cell.
- **Tidak Ada Hasil**: Pastikan ejaan nama perusahaan sudah benar dan coba gunakan keyword yang lebih spesifik.
- **Proses Lambat/Timeout**: Kinerja sangat bergantung pada koneksi internet. Jika gagal, coba dengan jumlah keyword yang lebih sedikit.
- **Optimisasi**: Untuk menghemat memori, bersihkan data (`🗑️ Bersihkan`) setelah melakukan ekspor.

## ⚖️ Etika & Penafian

- Tool ini dibuat untuk tujuan **edukasi dan penelitian**.
- Harap gunakan secara bertanggung jawab dan hormati **Terms of Service** dari JobStreet.
- Tool ini memiliki jeda waktu antar permintaan untuk tidak membebani server target.

## 👨‍💻 Author

- **Ferdian Bangkit Wijaya**
- Universitas Sultan Ageng Tirtayasa (UNTIRTA)
- Versi: 1.0.0 (Agustus 2025)

---

> Proyek ini didedikasikan untuk analisis dan riset lanskap perusahaan di Indonesia melalui data publik.
