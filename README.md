# Microtech: Website E-Commerce Toko Komputer

> **Solusi Komputasi & Jaringan Terpercaya**

Microtech adalah rancangan antarmuka website e-commerce untuk toko komputer, laptop, sparepart, dan perangkat jaringan. Proyek ini merupakan Tugas Akhir **Asistensi Pengantar Teknologi Informasi (TC001B)**, Program Studi Teknik Informatika, Fakultas Teknologi Informasi, Universitas Kristen Satya Wacana (2026), oleh **Kelompok Ujang Kedu**.

> [!NOTE]
> Proyek ini adalah **front-end statis** tanpa backend dan database. Login, keranjang, dan pembayaran hanya simulasi tampilan. Data produk, harga, statistik, testimoni, dan profil perusahaan bersifat contoh untuk keperluan tugas.

## Daftar Isi

- [Tujuan](#tujuan)
- [Fitur Antarmuka](#fitur-antarmuka)
- [Teknologi](#teknologi)
- [Halaman](#halaman)
- [Alur Navigasi](#alur-navigasi)
- [Desain](#desain)
- [Struktur Proyek](#struktur-proyek)
- [Cara Menjalankan](#cara-menjalankan)
- [Keterbatasan](#keterbatasan)
- [Kontribusi](#kontribusi)
- [Developer Team](#developer-team)
- [Referensi](#referensi)

## Tujuan

Menghasilkan antarmuka yang modern, sederhana, rapi, informatif, dan mudah diakses oleh mahasiswa, penggemar teknologi, programmer, serta masyarakat umum.

## Fitur Antarmuka

- Landing page dan beranda dengan carousel produk serta brand
- Tampilan login, register, dan lupa password
- Katalog kategori, daftar produk, dan detail spesifikasi
- Tampilan keranjang, pembayaran, dan bukti pembayaran
- Pengaturan akun dan daftar pesanan dengan tab status
- Menu profil dropdown dan navigasi yang menyesuaikan layar kecil

## Teknologi

| Teknologi | Kegunaan |
|---|---|
| HTML5 | Struktur halaman |
| CSS | Penyesuaian tampilan lewat atribut `style` dan sedikit tag `<style>` |
| [Bootstrap 5.3.3](https://getbootstrap.com/) (CDN) | Layout responsif dan komponen (navbar, carousel, dropdown, collapse, tab) |
| [Bootstrap Icons 1.11.3](https://icons.getbootstrap.com/) (CDN) | Ikon |
| JavaScript | Bootstrap Bundle, efek navbar saat scroll, dan efek hover gambar |
| Google Fonts | Orbitron, Inter, dan Montserrat |

Tidak memerlukan instalasi paket maupun proses build.

## Halaman

| File | Isi |
|---|---|
| `landing-page.html` | Halaman awal untuk pengunjung yang belum login |
| `login.html` | Login, register, dan lupa password |
| `index.html` | Beranda setelah login |
| `about.html` | Tentang Microtech, visi misi, brand, dan founder |
| `produk.html` | Katalog kategori produk |
| `isi-produk.html` | Daftar produk kategori Ether Routers |
| `detail-produk.html` | Detail dan spesifikasi hEX refresh |
| `keranjang.html` | Keranjang belanja |
| `pembayaran.html` | Data pembeli dan metode pembayaran |
| `bukti_pembayaran.html` | Konfirmasi pembelian |
| `pesanan_saya.html` | Daftar pesanan |
| `account.html` | Pengaturan akun |
| `contact.html` | Informasi kontak |

## Alur Navigasi

```text
landing-page → login → index → produk → isi-produk → detail-produk → pembayaran → bukti_pembayaran

Menu profil → account | pesanan_saya | keranjang | keluar (landing-page)
```

## Desain

Nama **Microtech** berasal dari *Micro* dan *Technology*: hal kecil yang dikelola lewat teknologi dan inovasi dapat menghasilkan perubahan besar. Nilai utamanya adalah ketelitian, inovasi, efisiensi, kemajuan, dan kesederhanaan.

**Prinsip UI/UX**

- **Usability:** tata letak dan navigasi sederhana.
- **Visual Hierarchy:** informasi penting ditonjolkan lewat ukuran, warna, dan posisi.
- **Consistency:** warna, tipografi, tombol, dan tata letak diseragamkan.

**Tipografi**

- **Orbitron:** judul, menu, dan nama produk
- **Inter:** teks deskripsi
- **Montserrat:** halaman login

**Warna utama**

| Warna | Kode |
|---|---|
| Merah marun | `#7A0C12` |
| Merah | `#C00000` |
| Biru gelap (gradasi footer) | `#14102B` |
| Putih | `#FFFFFF` |

## Struktur Proyek

```text
.
├── assets/
│   ├── account/
│   ├── beranda/
│   ├── bukti_pembayaran/
│   ├── dropdown/
│   ├── ether-routers/
│   ├── keranjang/
│   ├── kontak/
│   ├── landing_page/
│   ├── login/
│   ├── pesanan_saya/
│   ├── product/
│   └── tentang/
├── *.html
└── README.md
```

## Cara Menjalankan

1. Clone repository (versi stabil dari branch `main`):

   ```bash
   git clone -b main https://github.com/yosephnainggolan/Project_E-commerce_Ujang-Kedu.git
   cd Project_E-commerce_Ujang-Kedu
   ```

2. Buka `landing-page.html` di browser, atau gunakan ekstensi **Live Server** di VS Code.

Koneksi internet diperlukan karena Bootstrap, ikon, dan font dimuat dari CDN.

Untuk memperbarui salinan yang sudah ada:

```bash
git switch main
git pull origin main
```

## Keterbatasan

- Data formulir tidak disimpan atau diverifikasi.
- Jumlah barang, total belanja, dan status pesanan tidak dihitung secara dinamis.
- Kartu produk mengarah ke halaman contoh yang sama.

## Kontribusi

| Branch | Fungsi |
|---|---|
| `test` | Perbaikan dan pengujian |
| `main` | Versi stabil |

**Tim pengembang**

```bash
git switch test
git pull --no-rebase origin test

# edit dan uji kode

git add .
git status
git commit -m "Deskripsi singkat perubahan"
git pull --no-rebase origin test
git push origin test
```

Setelah dipastikan aman, buat **Pull Request** dari `test` ke `main` untuk direview sebelum di-merge.

**Kontributor luar:** fork repository ini, lalu ajukan Pull Request ke branch `test`.

## Developer Team

| Nama | Peran | Profil |
|---|---|---|
| Yoseph Immanuel Nainggolan | Chief Executive Officer | [LinkedIn](https://www.linkedin.com/in/yoseph-immanuel-nainggolan/) · [GitHub](https://github.com/yosephnainggolan) |
| Jesen Marselino Pakpahan | Chief Software Development | [LinkedIn](https://www.linkedin.com/in/jesen-marselino-270bab35a/) · [GitHub](https://github.com/jesenmars77) |
| Matthew Sequaia Marvino Metekohy | Chief UI/UX Designer | [LinkedIn](https://www.linkedin.com/in/matthew-metekohy-0a1b10451/) · [GitHub](https://github.com/mattewajadeh) |
| Septuaginta Clea Gavrila Barthimeus | Chief AI Consultant | [LinkedIn](https://www.linkedin.com/in/septuaginta-clea-7669b6451) · [GitHub](https://github.com/cleallvr) |

## Referensi

- [Web Programming UNPAS](https://wpucourse.id)
- [MikroTik](https://mikrotik.com)
