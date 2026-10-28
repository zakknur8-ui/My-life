ROAD TO 2030 — LIFE RPG

Isi folder:
- index.html: aplikasi Road to 2030 dengan fitur life RPG dan jurnal
- manifest.json: metadata PWA
- sw.js: service worker cache offline (cache versi baru)
- icon-192.png dan icon-512.png: ikon aplikasi

FITUR:
- Beranda dan roadmap checklist 2026–2030
- Daily Quest dan Weekly Quest dengan XP, level, streak, dan achievement
- Training Quest 4 hari/minggu: program otomatis Upper A, Lower A, Upper B, Lower B
- Jadwal latihan bisa diganti dengan memilih satu hari terjadwal lalu hari penggantinya
- Home gym: barbel, bench/rack, lat pulldown; tidak ada deadlift wajib
- Character Status: Finance, Body, Japanese, Career, Mind
- Financial Roadmap dengan tabungan saat ini, target, tabungan bulanan, dan estimasi waktu
- Consistency Map / kalender aktivitas
- Milestone pribadi
- Jurnal dengan timestamp Jepang (JST), riwayat scroll, edit, hapus, dan salin
- Time Capsule dengan tanggal buka
- Backup dan pemulihan JSON untuk semua data

PENTING TENTANG DATA:
Aplikasi menggunakan localStorage dengan key `road2030`, sama seperti versi sebelumnya. Jika memperbarui file pada URL/host yang sama, data lokal di browser seharusnya tetap ada. Namun, sebelum mengganti file, ekspor backup JSON dari versi lama terlebih dahulu. Jangan menghapus data browser atau data situs.

Time Capsule hanya menyembunyikan isi melalui antarmuka sampai tanggal yang dipilih; ini bukan enkripsi. Jangan simpan kata sandi atau informasi sangat sensitif di dalamnya.

CARA MEMPERBARUI DI GITHUB PAGES:
1. Buka aplikasi versi lama dan masuk ke menu Data.
2. Tekan “Unduh cadangan lengkap (.json)” untuk membuat backup.
3. Ekstrak ZIP ini.
4. Upload/ganti seluruh file di root repository GitHub Pages dengan file dari folder `road-to-2030` (termasuk index.html, manifest.json, sw.js, dan ikon).
5. Tunggu deployment selesai, lalu buka URL aplikasi yang sama.
6. Jika tampilan masih versi lama, tutup aplikasi/PWA sepenuhnya lalu buka kembali. Service worker cache sudah dinaikkan versinya.
7. Jika data tidak terlihat, jangan langsung reset. Coba pulihkan backup JSON yang dibuat di langkah 2.

Aplikasi menyimpan data secara lokal dan tidak otomatis sinkron antarperangkat.
