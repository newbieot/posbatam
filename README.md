# Landing Page Layanan Pos Indonesia

Website statis responsif untuk mempromosikan layanan:

- Kiriman Kargo
- Kendaraan Bermotor
- Barang Pindahan
- Kontak PIC: Ricky Djuliandri — 081372212002
- QR code informasi layanan

## Struktur

```text
posind-landing-page/
├── index.html
├── styles.css
├── script.js
├── _headers
├── 404.html
└── assets/
    ├── danantara-logo.webp
    ├── posind-logo.svg
    ├── hero-logistics.png
    ├── qr-posind.png
    └── favicon.svg
```

## Menjalankan di komputer

Buka `index.html` langsung di browser, atau gunakan server lokal:

```bash
python -m http.server 8080
```

Lalu buka `http://localhost:8080`.

## Deploy ke GitHub

1. Buat repository baru di GitHub.
2. Upload seluruh isi folder ini ke repository.
3. Pastikan `index.html` berada di direktori paling atas repository.

## Hubungkan ke Cloudflare Pages

1. Masuk ke Cloudflare Dashboard.
2. Buka **Workers & Pages** → **Create** → **Pages**.
3. Pilih **Connect to Git** dan hubungkan repository GitHub.
4. Gunakan pengaturan:
   - Framework preset: `None`
   - Build command: kosong
   - Build output directory: `/`
5. Klik **Save and Deploy**.

## Mengubah data

- Nomor WhatsApp/PIC: cari `081372212002` pada `index.html`.
- Nama PIC: cari `Ricky Djuliandri` pada `index.html`.
- QR code: ganti `assets/qr-posind.png` dengan file QR baru memakai nama yang sama.
- Logo: ganti file di folder `assets` dan pertahankan nama file agar tidak perlu mengubah HTML.

> Catatan: pastikan penggunaan logo dan materi promosi telah sesuai izin serta pedoman identitas merek yang berlaku.
