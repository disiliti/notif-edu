# notif-edu (PWA)

Aplikasi web sederhana untuk membuat pengingat Google Calendar (jam 11:00 WIB, berulang tiap 6 hari x4) dengan daftar nama tersimpan (localStorage). Sudah siap **PWA** (bisa di-install di Android).

## Struktur
```
notif-edu/
├─ index.html
├─ manifest.webmanifest
├─ sw.js
├─ icons/
│  ├─ icon-192.png
│  └─ icon-512.png
└─ .nojekyll
```

## Deploy cepat ke GitHub Pages
1. Aktifkan GitHub Pages: **Settings → Pages → Build and deployment → Deploy from branch**.  
   Pilih **Branch: main** dan **Folder: /(root)** → Save.
2. Commit & push berkas di atas ke repo.
3. Akses situs di URL GitHub Pages repo kamu (format: `https://<username>.github.io/<repo>/`).

## Tambah ke Google Calendar
- Isi nama & tanggal mulai → klik **Tambah ke Google Calendar**.  
- Judul otomatis: `{NAMA} ISI PAKE EDU!!`. Durasi 60 menit (11:00–12:00 WIB).  
- Pola pengulangan: `RRULE:FREQ=DAILY;INTERVAL=6;COUNT=4`.

## Catatan
- Nama yang pernah dipakai disimpan lokal di browser (tidak ke server).
- App bisa di-install (Chrome Android) karena PWA (manifest + service worker).
