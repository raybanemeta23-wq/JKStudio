# Cara Install AromaCraft di HP (Android & iPhone) — Tanpa App Store

App ini sekarang sudah jadi **PWA (Progressive Web App)**: bisa diinstall langsung ke
Android dan iPhone dari browser, tampil seperti app biasa (ikon di homescreen, full
screen tanpa address bar), dan tetap bisa dibuka walau tanpa internet — semua **gratis**,
tanpa akun developer, tanpa proses review.

## Langkah 1 — Upload ke hosting gratis (wajib)

PWA butuh diakses lewat **HTTPS** supaya bisa diinstall dengan benar (terutama untuk
service worker dan tombol "Install" di Chrome). Cara paling gampang dan gratis:

### Opsi A — Netlify Drop (paling simpel, tanpa akun)
1. Buka https://app.netlify.com/drop di browser komputer
2. Drag & drop folder `www` (isi folder ini, bukan foldernya) ke halaman itu
3. Netlify langsung kasih link seperti `https://nama-acak.netlify.app`
4. Buka link itu di HP kamu

### Opsi B — GitHub Pages (kalau sudah punya akun GitHub)
1. Buat repo baru, upload semua isi folder `www`
2. Masuk ke Settings > Pages > Deploy from branch > pilih `main` / root
3. Link jadi `https://username.github.io/nama-repo`

### Opsi C — Vercel
1. https://vercel.com, sign up gratis, drag & drop folder `www` lewat dashboard "Add New Project"

## Langkah 2 — Install di Android (Chrome)
1. Buka link hosting kamu di Chrome
2. Ketuk menu titik tiga (⋮) di pojok kanan atas
3. Pilih **"Install app"** atau **"Tambahkan ke layar Utama"**
4. Ikon AromaCraft akan muncul di homescreen, terbuka full screen seperti app native

## Langkah 3 — Install di iPhone (Safari — wajib pakai Safari, bukan Chrome)
1. Buka link hosting kamu di **Safari**
2. Ketuk ikon **Share/Bagikan** (kotak dengan panah ke atas) di bagian bawah
3. Scroll dan pilih **"Add to Home Screen" / "Tambah ke Layar Utama"**
4. Ketuk **"Add"** di pojok kanan atas
5. Ikon AromaCraft akan muncul di homescreen, terbuka full screen tanpa address bar

## Catatan
- Ini **bukan** file APK atau IPA yang diinstall lewat file — ini web app yang "dibungkus"
  jadi terasa seperti app native di homescreen. Tidak perlu izin "unknown sources", tidak
  perlu akun developer, dan bisa langsung dibagikan ke siapa saja tinggal kirim link.
- Data Jurnal Resep tersimpan di `localStorage` per-device — kalau user hapus cache
  browser atau ganti HP, data itu tidak ikut pindah.
- Kalau nanti kamu mau upgrade ke app "beneran" yang bisa didownload dari Google Play /
  App Store (dengan ikon APK/IPA asli), project Capacitor yang saya buatkan sebelumnya
  bisa dipakai lagi kapan saja — tinggal bilang.
