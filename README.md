# Temu — Prototipe QR Event

Website statis HTML, CSS, dan JavaScript. Tidak memerlukan npm, server aplikasi, atau proses build.

## Publikasi ke GitHub Pages

1. Ekstrak ZIP ini.
2. Buat repository GitHub, misalnya `temu-event`. Untuk GitHub Free gunakan repository Public.
3. Upload seluruh isi hasil ekstraksi langsung ke root repository, bukan ZIP-nya dan bukan folder pembungkus. Pastikan `index.html` terlihat di halaman utama repository.
4. Commit ke branch `main`.
5. Buka Settings → Pages → Build and deployment.
6. Pilih Source: Deploy from a branch; Branch: main; folder: /(root); klik Save.
7. Tunggu proses deployment selesai. Buka alamat yang ditampilkan di Settings → Pages.
8. Buat/cetak QR dari halaman yang sudah dipublikasikan agar QR memakai alamat GitHub Pages Anda.

Dokumentasi resmi: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Uji alur

- Pilih Undangan & QR → Andi Pratama → Coba tampilan tamu.
- Kembali ke Registrasi → cari TM001 → Buka → atur pendamping → Konfirmasi hadir.
- Buka tamu yang sama untuk melihat status sudah hadir.
- Coba tamu tambahan dan kapasitas meja (8 orang per meja).
- Ekspor CSV untuk dibuka/import di Google Sheets. Menu Cara mencoba menyediakan reset data.

## Batas prototipe

- Hanya untuk simulasi dengan data fiktif; belum memiliki login atau otorisasi petugas.
- Data tersimpan di localStorage browser, tidak tersinkron antarperangkat dan tidak terhubung langsung ke Google Sheets.
- QR berisi salinan nama dan alokasi, bukan token aman. Buat ulang setelah perubahan meja/kursi.
- Membuka halaman tamu tidak mencatat kehadiran; petugas mengonfirmasi melalui registrasi.
- Pindai kamera tergantung dukungan BarcodeDetector dan izin kamera di browser. Gunakan pencarian kode jika tidak tersedia.
- Tamu tambahan yang dibuat di satu browser tidak otomatis tersedia untuk registrasi di browser lain.
- Ekspor CSV adalah snapshot, bukan cadangan yang bisa diimpor kembali melalui aplikasi ini.

## Isi

- index.html: halaman aplikasi
- style.css: tampilan responsif dan cetak
- app.js: logika simulasi
- qrcode.js: QR Code Generator oleh Kazuhiko Arase, berlisensi MIT (atribusi pada file)

Versi ekspor ini menyesuaikan keterangan akses untuk GitHub Pages. Situs demo sebelumnya tidak diubah.
