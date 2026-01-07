Indie Press Studio

"Sistem Penerbitan Mandiri Tanpa Backend. Tulis, Edit, Terbitkan."

Indie Press Studio adalah aplikasi web single-page (SPA) yang dirancang untuk penulis yang menginginkan kontrol penuh atas karya mereka tanpa gangguan sistem manajemen konten (CMS) yang rumit. Aplikasi ini berjalan sepenuhnya di browser (Client-Side), menyimpan data secara lokal, dan mampu mengekspor naskah menjadi Ebook (HTML) siap baca.

🔥 Fitur Utama

1. Manajemen Perpustakaan (Storefront)

Tampilan rak buku visual dengan sampul 3D interaktif.

Filter otomatis berdasarkan Genre (Fiksi, Non-Fiksi, dll).

Pencarian real-time untuk Judul dan Penulis.

2. Studio Penulisan (The Writer's Room)

Rich Text Editor: Dukungan penuh untuk Bold, Italic, Underline, Heading, dan Blockquote. Bukan sekadar textarea polos.

Word Counter: Penghitung kata otomatis per bab untuk menjaga target penulisan.

Manajemen Bab: Tambah, hapus, dan navigasi antar bab dengan mudah.

3. Metadata & Kustomisasi

Input URL Gambar untuk Sampul Buku kustom.

Pengaturan detail: Judul, Penulis, Sinopsis, dan Genre.

Mode Baca (Reader Mode) dengan opsi tema (Light, Sepia, Dark) dan ukuran font.

4. Keamanan & Ekspor Data

Zero-Backend: Data disimpan di localStorage browser pengguna. Privasi 100%.

Backup System: Ekspor seluruh perpustakaan ke format .JSON dan Impor kembali untuk memindahkan data antar perangkat.

Ebook Export: Unduh naskah final sebagai file .html terformat yang bersih (siap konversi ke PDF/EPUB).

🚀 Cara Penggunaan

Instalasi Lokal

Karena aplikasi ini zero-dependency, Anda tidak perlu npm install atau server lokal.

Clone repositori ini atau download file index.html.

Buka index.html langsung di browser modern (Chrome, Edge, Firefox, Safari).

Selesai. Studio siap digunakan.

Deployment (Online)

Untuk akses lintas perangkat, sangat disarankan menggunakan GitHub Pages:

Upload index.html ke repositori GitHub (pastikan nama file tepat index.html).

Masuk ke Settings > Pages.

Pilih Branch: main, Folder: / (root).

Klik Save. Situs Anda akan online dalam hitungan menit.

🛠️ Arsitektur Teknis

Aplikasi ini dibangun dengan filosofi Minimalisme Radikal:

HTML5: Struktur semantik.

Tailwind CSS (via CDN): Utilitas styling responsif dan tipografi.

Phosphor Icons: Ikonografi vektor yang tajam.

Vanilla JavaScript: Logika aplikasi inti (tanpa React/Vue/Angular) untuk performa maksimal dan ukuran file minimal.

LocalStorage API: Database NoSQL sederhana di sisi klien.

Struktur Data (JSON Schema)

Setiap buku disimpan dengan struktur objek berikut:

{
  "id": 1709283921,
  "title": "Judul Buku",
  "author": "Nama Penulis",
  "coverUrl": "https://...",
  "chapters": [
    {
      "title": "Bab 1",
      "content": "<p>Isi bab dengan format HTML...</p>"
    }
  ]
}


⚠️ Catatan Penting (Disclaimer)

Persistensi Data: Karena menggunakan localStorage, data Anda akan hilang jika Anda melakukan "Clear Cache/Browsing Data" pada browser.

Solusi: Selalu gunakan fitur Backup Data (Ikon Download) di pojok kanan atas secara berkala untuk mengamankan naskah Anda ke dalam file .json di komputer Anda.

Gambar Sampul: Aplikasi tidak menyimpan file gambar (blob) untuk menghemat ruang penyimpanan browser. Gunakan URL gambar yang valid (public link).

🤝 Kontribusi

Proyek ini Open Source. Jika Anda ingin menambahkan fitur (misalnya: integrasi Google Drive atau Export PDF langsung), silakan lakukan Fork dan Pull Request.

Dibuat dengan dedikasi untuk para penulis yang menolak kerumitan.
