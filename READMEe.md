
# Bookshelf API - Documentation

Bookshelf API adalah sebuah RESTful API yang digunakan untuk mengelola data buku, termasuk menambahkan, melihat, mengubah, dan menghapus buku.

---

## Persyaratan Sistem
Sebelum menjalankan aplikasi ini, pastikan Anda telah menginstal perangkat lunak berikut:
- **Node.js** (v14.x atau lebih baru): [Download dan Instal Node.js](https://nodejs.org/)
- **Postman** (untuk pengujian API): [Download dan Instal Postman](https://www.postman.com/downloads/)

---

## Langkah-Langkah Instalasi dan Menjalankan Aplikasi

1. **Clone atau Unduh Repository**
   ```bash
   git clone <URL-repository-anda>
   cd <folder-repository-anda>
   ```

2. **Instal Dependencies**
   Jalankan perintah berikut untuk menginstal semua dependensi yang diperlukan:
   ```bash
   npm install
   ```

3. **Menjalankan Server**
   Jalankan server dengan perintah berikut:
   ```bash
   node server.js
   ```
   Anda akan melihat output berikut jika server berjalan dengan benar:
   ```
   Server berjalan pada http://localhost:9000
   ```

---

## Pengujian API dengan Postman

1. **Import File Collection dan Environment ke Postman**:
   - Import file `Bookshelf API Test.postman_collection.json` dan `Bookshelf API Test.postman_environment.json` ke dalam Postman.
   - Pastikan environment `Bookshelf API Test` aktif.

2. **Pengujian Endpoint**:
   - Gunakan Postman untuk menguji setiap endpoint, seperti:
     - **POST**: Tambah Buku  
       URL: `http://localhost:9000/books`
     - **GET**: Ambil Semua Buku  
       URL: `http://localhost:9000/books`
     - **GET**: Ambil Buku Berdasarkan ID  
       URL: `http://localhost:9000/books/{bookId}`
     - **PUT**: Ubah Buku Berdasarkan ID  
       URL: `http://localhost:9000/books/{bookId}`
     - **DELETE**: Hapus Buku Berdasarkan ID  
       URL: `http://localhost:9000/books/{bookId}`

---

## Struktur Folder dan File

```
/project-root
│
├── books.js                   # Data penyimpanan sementara untuk buku
├── handler.js                 # Handler untuk setiap route
├── routes.js                  # Definisi route untuk API
├── server.js                  # Konfigurasi dan inisialisasi server
├── Bookshelf API Test.postman_collection.json  # File collection Postman
├── Bookshelf API Test.postman_environment.json # File environment Postman
└── README.md                  # Dokumentasi proyek ini
```

---

## Catatan Tambahan
- Pastikan tidak ada aplikasi lain yang menggunakan port **9000** saat menjalankan server ini.
- Jika Anda ingin menggunakan port yang berbeda, ubah konfigurasi port di `server.js` dan sesuaikan environment Postman.

---

## Lisensi
Proyek ini dilisensikan di bawah lisensi MIT.

