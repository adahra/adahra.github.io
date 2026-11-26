# adahra.github.io

Situs pribadi statis milik Adnanto A.R. — Flutter Developer & Linux Enthusiast. Situs menampilkan profil, keterampilan teknis, proyek terpilih, dan kontak, dibangun dengan Hugo dan dihosting di GitHub Pages.

## Fitur Utama

- Halaman beranda (hand-edited) dengan hero, about, skills, projects, dan contact
- Halaman daftar postingan (`posts/`) dan RSS feed (`posts/index.xml`)
- Halaman kategori (`categories/`) dan tag (`tags/`) dengan RSS feed masing-masing
- Berkas RSS utama (`index.xml`) dan peta situs (`sitemap.xml`)
- Halaman 404 kustom (`404.html`)
- Aset CSS TACHYONS v4.9.1 yang dihash di `dist/css/` dan satu bundle JS di `dist/js/`
- Open Graph dan Twitter Card meta tag di setiap halaman
- Lisensi GPL v2 pada berkas yang diedit secara manual (mis. `index.html`)

Situs ini adalah output build statis saja. Sumber Hugo (`content/`, `layouts/`, `config.toml`) dan alat build tidak ada di repository ini.

## Prasyarat & Cara Instalasi

Tidak diperlukan penginstalan dependensi. Repository berisi hanya berkas statis (HTML, CSS, JS, XML, gambar) yang siap disajikan oleh web server statis apa pun (mis. GitHub Pages).

## Konfigurasi

Tidak ada berkas konfigurasi maupun variabel environment di repository ini. Konfigurasi asli (Hugo `config.toml`) dikelola di proyek sumber eksternal dan tidak tersimpan di sini.

## Cara Menjalankan & Testing

Tidak ada perintah build, pengujian, atau paket manajer di repository ini. Untuk menyajikan secara lokal, cukup ajak berkas statis, contoh:

```bash
python3 -m http.server 8000
```

Buka `http://localhost:8000` di browser.

Untuk me-regenerasi situs, gunakan proyek sumber Hugo secara eksternal:

```bash
hugo --minify
```

## Struktur Direktori Utama

| Jalur | Keterangan |
|---|---|
| `index.html` | Halaman beranda (diedit secara manual, berisi inline style dan header GPL v2) |
| `404.html` | Halaman 404 kustom |
| `index.xml` | RSS feed utama |
| `sitemap.xml` | Peta situs untuk SEO |
| `posts/` | Daftar postingan (`index.html`), feed (`index.xml`), dan postingan contoh (`my-first-post/`) |
| `categories/` | Halaman kategori dan feed RSS |
| `tags/` | Halaman tag dan feed RSS |
| `images/` | Aset media |
| `dist/css/` | Berkas CSS TACHYONS yang dihash |
| `dist/js/` | Bundle JavaScript |
| `AGENTS.md` | Pedoman agen/repository |

Situs dihosting di GitHub Pages pada `adahra.github.io`, branch `master`.
