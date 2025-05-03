LAPORAN TEKNIS APLIKASI CHAT BERBASIS WEBSOCKET
1. Pendahuluan
Aplikasi ini merupakan sistem chat real-time yang dibangun menggunakan WebSocket dengan Node.js. Tujuan utama dari sistem ini adalah menyediakan komunikasi dua arah antara klien dan server tanpa perlu me-refresh halaman.

2. Teknologi yang Digunakan
Node.js: Platform server-side berbasis JavaScript.

ws (WebSocket): Library WebSocket untuk Node.js.

HTML/CSS: Untuk antarmuka pengguna di sisi klien.

JavaScript (browser): Untuk mengelola koneksi WebSocket dari klien.

3. Struktur Proyek
bash
Salin
Edit
websocket_chat/
├── client.html           # Antarmuka klien
├── server.js             # Server WebSocket
├── package.json          # Metadata dan dependensi
└── node_modules/         # Folder dependensi
4. Instalasi dan Menjalankan Aplikasi
a. Persyaratan
Node.js telah terinstal

b. Langkah-langkah
bash
Salin
Edit
cd websocket_chat
npm install
node server.js
Akses client.html menggunakan browser setelah server dijalankan (gunakan Live Server jika diperlukan).

5. Alur Kerja Sistem
Klien membuka client.html, yang akan mencoba terhubung ke server WebSocket.

Server menerima koneksi dan menunggu pesan dari klien.

Ketika pesan dikirim, server menyebarkannya ke semua klien yang terhubung.

Klien menerima dan menampilkan pesan secara real-time.
