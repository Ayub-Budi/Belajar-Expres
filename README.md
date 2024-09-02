# Backend Project

Ini adalah dokumentasi untuk proyek backend yang dibuat menggunakan Node.js dan Express.

## Persyaratan

- Node.js (disarankan versi terbaru)
- npm (disarankan versi terbaru)
- MySQL

## Instalasi

1. Clone repository ini:

   ```bash
   git clone <URL_REPOSITORY_ANDA>
   cd <NAMA_FOLDER_PROJECT>
   ```

2. Instal dependensi yang diperlukan:

   ```bash
   npm install
   ```

3. Buat file `.env` di root proyek Anda dan isikan dengan konfigurasi berikut:

   ```plaintext
   DATABASE_URL="mysql://root:@localhost:3306/db_express"
   ```

4. Untuk keamanan, Anda perlu menghasilkan kode rahasia untuk JWT. Jalankan perintah berikut untuk membuatnya:

   ```bash
   node -e "console.log(require('crypto').randomBytes(32).toString('hex'))"
   ```

   Salin hasil yang dihasilkan dan tambahkan ke file `.env`:

   ```plaintext
   JWT_SECRET=paste_kode_random_hasil_generate_sebelumnya
   ```

## Menjalankan Proyek

Untuk menjalankan proyek ini secara lokal, gunakan perintah berikut:

```bash
nodemon index.js
```

Nodemon akan secara otomatis memantau perubahan di file dan merestart server jika diperlukan.

## License

Proyek ini dilisensikan di bawah lisensi MIT. Lihat file [LICENSE](LICENSE) untuk informasi lebih lanjut.
