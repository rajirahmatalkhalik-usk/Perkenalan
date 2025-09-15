# Website Perkenalan

Website ini dibangun menggunakan **HTML** dan **CSS** dengan tampilan
sederhana namun interaktif. Fitur yang digunakan mencakup navigasi
responsif, tata letak berbasis card, serta penggunaan *checkbox hack*
untuk menghadirkan interaktivitas tanpa memerlukan JavaScript.

🔗 **Demo Website**: [Kunjungi
Website](https://rajirahmatalkhalik-usk.github.io/Perkenalan/index.html)

------------------------------------------------------------------------

## Struktur Direktori

    .
    ├── index.html       # Halaman Profil
    ├── data.html        # Halaman Data Akademik & Sikap Belajar
    ├── styles.css       # Berkas CSS untuk styling
    ├── assets/          # Folder aset (ikon, gambar, background)

------------------------------------------------------------------------

## Deskripsi Halaman

### 1. `index.html`

Menampilkan informasi profil berupa:
- Foto profil
- Nama dan NPM
- Deskripsi singkat mengenai identitas umum

### 2. `data.html`

Berisi informasi akademik dalam bentuk:
- **Tabel** data akademik (NPM, Program Studi, Angkatan, Fokus Belajar)
- **Daftar** sikap belajar

### 3. `styles.css`

Mengatur tampilan antarmuka, meliputi:
- **Layout responsif** dengan Flexbox dan Media Query
- **Navigasi interaktif** dengan hamburger menu
- **Card layout** untuk konten utama
- Opsi mode tampilan (Terang/Gelap) --- *masih dalam tahap pengembangan*

------------------------------------------------------------------------

## Fitur Teknis

-   **Responsif**: Mendukung perangkat desktop dan mobile.
-   **Navigasi Dinamis**: Menggunakan metode *checkbox hack* untuk mengatur menu.
-   **Hamburger Menu**: Tampil otomatis pada resolusi layar kecil.
-   **Submenu Tampilan**: Pilihan mode terang dan gelap.

------------------------------------------------------------------------

## Contoh Sintaks Interaktif

Salah satu fitur menarik pada website ini adalah penggunaan elemen
**`<input type="checkbox">`** yang dikombinasikan dengan CSS untuk
menghadirkan fungsi interaktif tanpa JavaScript.

### Contoh: Hamburger Menu

``` html
<!-- Checkbox untuk toggle -->
<input type="checkbox" id="menu-toggle">
<label for="menu-toggle" class="menu-btn">
  <span></span>
  <span></span>
  <span></span>
</label>

<!-- Menu Navigasi -->
<nav class="menu-main">
  <a href="index.html">Profil</a>
  <a href="data.html">Data</a>
</nav>
```

### CSS Pendukung:

``` css
/* Default: menu disembunyikan */
.navigation nav {
  display: none;
}

/* Saat checkbox dicentang, tampilkan menu */
#menu-toggle:checked ~ nav {
  display: block;
}
```

👉 Dengan teknik ini, interaksi sederhana seperti membuka/menutup menu
dapat dicapai tanpa JavaScript.

------------------------------------------------------------------------

## Cara Menjalankan

1.  Clone repository:

    ``` bash
    git clone https://github.com/rajirahmatalkhalik-usk/Perkenalan.git
    ```

2.  Masuk ke direktori proyek:

    ``` bash
    cd Perkenalan
    ```

3.  Buka `index.html` menggunakan browser.

------------------------------------------------------------------------

## Catatan

-   Fitur **dark mode** masih dalam tahap pengembangan (kode CSS
    dikomentari).
-   Pastikan direktori `assets/` berisi gambar dan ikon untuk mendukung
    tampilan website.

------------------------------------------------------------------------

## Lisensi

Proyek ini dirilis sebagai contoh website statis dengan HTML dan CSS.
Konten dapat digunakan dan dimodifikasi secara bebas untuk tujuan
pembelajaran maupun pengembangan lebih lanjut.
