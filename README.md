# Platform Web Interaktif ITENAS 2026

## Tentang Proyek
--------------------------------------------------------------------------------

## Tugas ini merupakan Deliverable untuk pertemuan Tugas p4 dan Evaluasi 1


Proyek ini adalah aplikasi web interaktif yang menggabungkan beberapa modul fungsional dalam satu dashboard terpadu.
---

## Modul-Modul Utama

###  Beranda Utama (`index.html`)
Halaman selamat datang yang berfungsi sebagai pintu masuk ke sistem.

**Komponen:**
- Layout header dengan galeri gambar
- Navigasi sidebar yang dapat diakses dari semua halaman
- Tombol interaktif yang menampilkan pesan sambutan

---

###  Kasir Restoran (`menu.html`)
Simulasi sistem penjualan point-of-sale (POS) untuk restoran dengan perhitungan otomatis.

**Menu Makanan:**
| Produk | Harga |
|--------|-------|
| Mie Ayam | Rp 12.000 |
| Lontong Kari | Rp 11.000 |
| Spagethi Jumbo | Rp 17.000 |

**Fitur Utama:**
-  Sistem input kuantitas real-time
-  Perhitungan total otomatis
-  Diskon cerdas: 10% untuk pembelian >Rp 50.000
-  Validasi input (mencegah angka negatif)
-  Button reset untuk membersihkan form

**Alur Kerja:**
1. Masukkan jumlah pesanan untuk setiap item
2. Sistem otomatis menghitung total harga
3. Jika total >Rp 50.000, diskon 10% diterapkan
4. Lihat ringkasan final dan total pembayaran

---

###  Kalkulator Ilmiah (`calculator.html`)
Aplikasi kalkulator sederhana untuk operasi matematika dasar.

**Operator Tersedia:**
-  Penjumlahan (`+`)
-  Pengurangan (`-`)
-  Perkalian (`*`)
-  Pembagian (`/`)
-  Modulo (`%`)
-  Perpangkatan (`^`)

**Keamanan Input:**
- Tidak boleh ada input kosong
- Nilai harus lebih besar dari 0
- Alert otomatis jika terjadi kesalahan

---

###  Program Garis Hidup (`garis_hidup.html`)
Program numerologi yang menganalisis kepribadian berdasarkan tanggal lahir menggunakan konsep Life Path Number.

**Cara Kerja:**
```
Input: Tanggal, Bulan, Tahun Lahir
        ↓
Gabungkan semua angka
        ↓
Jumlahkan setiap digit secara berulang
        ↓
Hasil akhir: Satu angka (1-9)
```

**Contoh Perhitungan:**
```
Lahir: 15 Maret 1998
→ 1+5+3+1+9+9+8 = 36
→ 3+6 = 9
→ Garis Hidup: 9
```

**Output:**
- Tabel hasil perhitungan (proses step-by-step)
- Angka garis hidup final (1-9)
- Penjelasan karakter berdasarkan numerologi

---

##  Teknologi yang Digunakan

| Teknologi | Fungsi |
|-----------|--------|
| **HTML5** | Struktur dan semantik halaman |
| **CSS3** | Styling, layout (Flexbox, Grid), responsive design |
| **JavaScript ES6+** | Event handling, DOM manipulation, logika program |

---

##  Struktur Direktori

```
tugas4/
│
├── index.html              # Halaman utama
├── menu.html               # Modul kasir
├── calculator.html         # Modul kalkulator
├── garis_hidup.html        # Modul numerologi
│
├── css/
│   └── style.css           # Stylesheet terpadu untuk semua halaman
│
├── js/
│   └── script.js           # Logika JavaScript untuk semua modul
│
├── asset/
│   ├── logo-itenas.png     # Background logo
│   └── gedung.jpeg         # Header image
│
└── README.md               # File dokumentasi ini
```

---

##  Desain & UX

**Warna Tema:**
- Warna Primer: Oranye (#df9e28)
- Warna Sekunder: Ungu (#9330a8)
- Aksen: Kuning (#ffcc00), Biru (#5c7eb8)

**Konsistensi Antarmuka:**
- Sidebar navigasi yang unified
- Header dengan visual yang konsisten
- Footer dengan informasi identitas
- Responsive dan mobile-friendly

---

##  Cara Menggunakan

### Prasyarat
- Browser web modern (Chrome, Firefox, Safari, Edge)
- File dan folder struktur sudah sesuai

### Langkah-langkah

1. **Unduh/Clone Repository**
   ```bash
   git clone <repository-url>
   cd tugas4
   ```

2. **Buka di Browser**
   - Buka file `index.html` secara langsung, atau
   - Gunakan live server (VSCode Live Server Extension)

3. **Navigasi Antar Modul**
   - Klik menu di sidebar untuk berpindah antar halaman
   - Setiap modul dapat berdiri sendiri

---

##  Fitur Unggulan

 **Single-Page-Like Experience** - Navigasi mulus antar halaman  
 **Real-time Calculation** - Perhitungan otomatis tanpa refresh  
 **Input Validation** - Validasi data untuk keamanan  
 **Consistent Design** - UI/UX yang unified di semua halaman  
 **Lightweight** - Tanpa dependencies eksternal (vanilla JavaScript)  

---

##  Catatan Pengembang

- Semua logika frontend berjalan di client-side
- Tidak ada koneksi database atau backend server
- Event listeners digunakan untuk interaktivitas real-time
- CSS Grid dan Flexbox untuk layout responsif

---

##  Identitas Projekm

**NIM:** 162023032  
**Institusi:** ITENAS (Institut Teknologi Nasional)  
**Program Studi:** Sistem Informasi  
**Tahun:** 2026

---

## Lisensi

Proyek ini dibuat untuk tujuan pendidikan dan pengembangan skill praktis.

---

**Last Updated:** March 2026
