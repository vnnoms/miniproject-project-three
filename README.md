# TutorIn — Student Peer Learning Hub
Nama: Callista Rahma Putri
NIM: 251511004
Kelas: D3-1A Teknik Informatika
Mata Kuliah: Proyek Pengembangan Perangkat Lunak Berbasis Web (Proyek 3)
Institusi: Politeknik Negeri Bandung

TutorIn adalah sebuah *landing page* statis yang dirancang sebagai pusat kolaborasi dan bimbingan belajar antarmahasiswa (*peer-to-peer learning network*) di lingkungan Jurusan Teknik Komputer dan Informatika (JTK), Politeknik Negeri Bandung. Situs ini bertujuan menjembatani kesenjangan pemahaman logika pemrograman, bedah kode, dan standar rekayasa web bagi mahasiswa tingkat awal secara inklusif dan terstruktur.

---

## 🚀 Fitur Utama & Struktur Antarmuka

- **Hero Carousel Interaktif (Pure CSS):** Tata letak layar penuh yang terinspirasi dari antarmuka modern minimalis, memanfaatkan *CSS scroll-snap* dan tautan anchor ID untuk berpindah slide gambar tanpa ketergantungan JavaScript.
- **Arsitektur Semantik Terstruktur:** Mematuhi standar W3C dengan hierarki tepat satu `<h1>` pada bagian *hero*, penataan `<section>` berbasis tema, serta pemanfaatan elemen `<figure>` dan `<figcaption>` untuk konten multimedia yang kontekstual.
- **Desain Responsif (Mobile-First):** Tata letak fleksibel menggunakan modul Flexbox yang adaptif di berbagai ukuran layar (320 px hingga desktop), bebas dari kendala *horizontal overflow*.
- **Desain Aksesibel:** Mendukung navigasi penuh via papan ketik melalui indikator `:focus-visible` berkontras tinggi, pelengkap atribut `alt` deskriptif pada setiap media gambar, dan target sentuh tautan yang proporsional.
- **Sistem Token Desain CSS:** Pengelolaan palet warna konsisten (*Navy Blue, Sapphire, Warm Taupe, Champagne, Ivory*) dan tipografi berbasis token custom properties `:root`.

---

## 📂 Struktur Berkas Proyek

```text
miniproject-project-three/
├── assets/
│   ├── informatics-engineering.jpg
│   ├── informatics-engineering-1.jpg
│   └── informatics-engineering-2.jpg
├── styles/
│   ├── variables.css
│   └── style.css
├── index.html
├── LICENSE
└── README.md

## REFLECTIVE ESSAY
Pengerjaan proyek mandiri pada Modul 1 ini memberikan pemahaman mendalam bahwa membangun antarmuka web modern membutuhkan ketelitian arsitektural, bukan sekadar menumpuk elemen visual. Tantangan terbesar yang dihadapi dalam proses pengembangan ini adalah merekayasa komponen carousel interaktif pada bagian hero murni menggunakan HTML dan CSS tanpa memanfaatkan baris kode JavaScript sama sekali.

Pada tahap awal, sempat terjadi galat struktural yang cukup membingungkan di mana elemen seksi bersarang ganda tanpa penutup yang valid, mengakibatkan kontainer kartu konten di bawahnya ikut tertarik ke dalam koordinat absolut layar penuh. Melalui proses diagnosis mandiri menggunakan tab Elements dan Computed pada peramban DevTools, saya memahami pentingnya diagram pohon DOM yang bersih serta bagaimana penentuan properti position: absolute, position: relative, dan kalkulasi sumbu Flexbox saling memengaruhi alur dokumen.

Selain itu, implementasi CSS scroll-snap yang dikombinasikan dengan token variabel global :root mempertegas pentingnya pemisahan dependensi gaya secara modular. Saya belajar bahwa penulisan jalur berkas (relative path) dari dalam folder terisolasi menuntut pemahaman struktur direktori yang presisi agar terhindar dari galat 404 pada aset media. Aspek aksesibilitas juga menjadi fokus krusial, di mana setiap tombol kendali dan tautan navigasi wajib memiliki state interaksi yang kontras agar tetap nyaman dioperasikan oleh pengguna papan ketik. Secara keseluruhan, proyek ini membangun fondasi berpikir terstruktur dalam merancang situs web yang semantik, skalabel, efisien, dan ramah pengguna sebelum melangkah ke integrasi dinamis tingkat lanjut.