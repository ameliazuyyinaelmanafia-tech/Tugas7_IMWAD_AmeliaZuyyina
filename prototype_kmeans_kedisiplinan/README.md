# Sikap — Prototype Clustering Kedisiplinan Siswa

Prototype web sederhana untuk demo pengelompokan data absensi siswa menggunakan algoritma K-Means (k=3).

## Fitur
- Input nama siswa dan jumlah hadir, izin, sakit, alfa.
- Validasi input dan penanganan error.
- Empty state saat data kosong.
- Memuat dataset contoh (12 baris sintetis, bukan data penelitian).
- Proses clustering K-Means di browser.
- Ringkasan hasil cluster Baik, Cukup, Kurang.
- Ekspor hasil ke CSV.
- Penyimpanan lokal browser dengan `localStorage`.

## Teknologi
- Frontend: HTML, CSS, JavaScript.
- Backend: tidak digunakan pada versi prototype ini.
- Penyimpanan: `localStorage` pada browser.
- API: tidak digunakan.
- AI/ML: algoritma K-Means diimplementasikan dalam JavaScript.

## Cara menjalankan
1. Ekstrak ZIP.
2. Buka `index.html` menggunakan browser modern (Chrome/Edge/Firefox).
3. Klik **Muat data contoh** untuk mencoba data sintetis, atau masukkan data sendiri.
4. Klik **Jalankan K-Means** untuk melihat hasil.
5. Coba kondisi empty state dengan menghapus semua data; coba error handling dengan menjalankan clustering saat data kurang dari 3 siswa.

## Catatan penting
- Dataset contoh bersifat sintetis dan hanya untuk demonstrasi, bukan data penelitian nyata.
- K-Means menghasilkan cluster tanpa label. Prototype memberi label Baik/Cukup/Kurang dengan mengurutkan skor centroid sederhana `hadir - (izin + sakit + alfa)`. Metode pelabelan ini perlu ditinjau dan disepakati dengan pembimbing sebelum dipakai dalam skripsi.
- Inisialisasi centroid dibuat deterministik untuk demo, bukan implementasi K-Means++ formal.
- Belum ada backend, database server, autentikasi, atau API.
- Untuk laporan demo, gunakan screenshot asli dari aplikasi setelah dijalankan. Jangan menyatakan pengujian atau hasil penelitian telah dilakukan jika belum.
- Untuk GitHub: buat repository baru, lalu unggah `index.html` dan `README.md`.
