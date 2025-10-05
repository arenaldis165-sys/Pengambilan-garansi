# Situs Pengambilan Garansi

Situs sederhana untuk menerima pengajuan pengambilan garansi.

Fitur:
- Form pengambilan garansi (nama, telepon, email, produk, nomor seri, tanggal pengambilan, alamat, catatan)
- Unggah bukti (batas 2 MB)
- Backend Express menyimpan file ke /uploads dan entri ke submissions.json

Cara menjalankan (lokal):
1. Salin .env.example menjadi .env dan sesuaikan variabel jika ingin mengaktifkan email.
2. npm install
3. npm start

Env vars yang penting:
- PORT (opsional, default 3000)
- SMTP_HOST, SMTP_PORT, SMTP_USER, SMTP_PASS (opsional untuk notifikasi email)

Lisensi: MIT