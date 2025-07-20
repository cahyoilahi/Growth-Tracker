# Growth Tracker - Dasbor Analitik Pertumbuhan Media Sosial

Growth Tracker adalah aplikasi web modern yang dirancang untuk membantu brand atau individu melacak dan menganalisis pertumbuhan mereka di berbagai platform media sosial. Aplikasi ini menyediakan dasbor terpusat untuk memvisualisasikan data pengikut (followers) dan suka (likes) dari waktu ke waktu.

Aplikasi ini dibangun dengan arsitektur serverless menggunakan Firebase, membuatnya cepat, aman, dan mudah untuk di-deploy.

## ✨ Fitur Utama
Otentikasi Pengguna: Sistem pendaftaran dan login yang aman menggunakan username dan password.

Dasbor Terpusat: Tampilan ringkas untuk semua metrik pertumbuhan di satu halaman.

Pelacakan Multi-Platform: Kemampuan untuk memasukkan username dari Instagram, X (Twitter), dan TikTok.

Visualisasi Data: Grafik interaktif untuk menganalisis tren pertumbuhan pengikut dan suka dalam rentang waktu 7, 30, atau 90 hari.

Unduh Laporan: Fitur untuk mengunduh tampilan grafik sebagai file PDF.

Desain Responsif: Tampilan yang optimal di berbagai perangkat, dari desktop hingga mobile.

## 💻 Teknologi yang Digunakan
Proyek ini dibangun menggunakan teknologi modern untuk frontend dan backend.

Frontend
HTML5

Tailwind CSS: Untuk styling yang cepat, modern, dan responsif.

JavaScript (ES6 Modules): Untuk semua logika interaktif di sisi klien.

Chart.js: Untuk membuat grafik yang indah dan interaktif.

jsPDF & html2canvas: Untuk fungsionalitas ekspor ke PDF.

Backend & Infrastruktur
Firebase Authentication: Untuk menangani semua proses otentikasi pengguna (daftar, masuk, keluar).

Firestore Database: Database NoSQL untuk menyimpan data pengguna, profil media sosial, dan data pertumbuhan harian.

Firebase Hosting: Untuk men-deploy dan menghosting aplikasi web secara global dengan cepat.

(Rencana) Firebase Cloud Functions: Untuk menjalankan logika backend secara otomatis (misalnya, mengambil data dari API media sosial setiap hari).

## 🚀 Cara Menjalankan Proyek Secara Lokal
Untuk menjalankan proyek ini di komputer Anda, ikuti langkah-langkah berikut:

Clone Repositori (Jika sudah di GitHub)

git clone https://github.com/username-anda/nama-repositori.git
cd nama-repositori

Buat Proyek Firebase

Buka Firebase Console dan buat proyek baru.

Tambahkan aplikasi web baru ke proyek Anda.

Aktifkan Authentication (dengan metode Email/Password) dan Firestore Database.

Konfigurasi Kunci Firebase

Salin objek firebaseConfig dari pengaturan proyek Firebase Anda.

Buka file public/js/app.js.

Tempel konfigurasi Anda di bagian yang telah disediakan.

Atur Aturan Keamanan (Security Rules)

Di dasbor Firestore, buka tab Rules.

Ganti aturan yang ada dengan aturan yang sesuai untuk login dengan username (seperti yang ada di dokumentasi proyek).

Jalankan dengan Live Server

Buka folder proyek di Visual Studio Code.

Klik kanan pada file public/index.html.

Pilih "Open with Live Server".

## 📁 Struktur Direktori
Struktur proyek ini dirancang agar rapi dan mudah dikelola.

/
├── public/                     # Semua file yang akan di-deploy (frontend)

│   ├── index.html

│   ├── css/style.css

│   └── js/app.js

│

├── functions/                # (Opsional) Untuk kode backend Cloud Functions
 
│   └── index.js

│

├── firebase.json                # Konfigurasi untuk Firebase Hosting

├── .firebaserc                 # Konfigurasi proyek Firebase

└── README.md                    # Anda sedang membacanya



## 🔮 Langkah Selanjutnya
Proyek ini memiliki potensi besar untuk dikembangkan lebih lanjut. Beberapa langkah selanjutnya yang bisa diambil:

Implementasi Cloud Functions: Mengganti mockData dengan data asli yang diambil secara otomatis dari API resmi media sosial.

Menambahkan Platform Baru: Mengintegrasikan platform lain seperti YouTube, LinkedIn, atau Facebook Pages.

Analisis Lebih Dalam: Menambahkan metrik baru seperti engagement rate, jangkauan (reach), dan postingan paling populer.

Kustomisasi Dasbor: Memungkinkan pengguna untuk mengatur ulang atau memilih metrik yang ingin mereka lihat.
