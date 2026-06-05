# Sudo DevWorks Static Starter

Folder ini adalah hasil konversi awal dari `home.blade.php` menjadi static HTML untuk Cloudflare Pages.

## Sebelum publish

1. Ganti semua `62XXXXXXXXXXX` di `index.html` dengan nomor WhatsApp resmi format internasional tanpa tanda plus. Contoh: `62812xxxxxxx`.
2. Ganti `[Nomor WhatsApp]` di footer.
3. Ganti `[Email Bisnis]` di footer.
4. Masukkan logo final ke `assets/logo/sudo-devworks-logo-icon-transparent.png`.
5. Opsional: masukkan Open Graph image ke `assets/images/og-image.png`.
6. Test lokal:

```bash
cd sudo-devworks-static-starter
python -m http.server 8000
```

Lalu buka `http://localhost:8000`.

## Catatan

Versi ini memakai Tailwind CDN agar cepat siap upload. Untuk production final yang lebih optimal, compile Tailwind dari project Laravel/Vite, lalu ganti CDN dengan file CSS hasil build.
