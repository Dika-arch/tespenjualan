# Mobile Banking UI PWA

Folder ini siap upload ke GitHub Pages.

## Isi file
- `index.html` — tampilan website utama responsive HP
- `manifest.json` — konfigurasi PWA agar bisa dibuka standalone dari Home Screen
- `service-worker.js` — cache sederhana untuk mendukung PWA
- `icon-192.png` dan `icon-512.png` — icon aplikasi
- `.nojekyll` — memastikan GitHub Pages membaca file apa adanya

## Upload ke GitHub lewat terminal VSCode

```powershell
cd D:\Download\tesbri
Copy-Item -Path "LOKASI_FOLDER_HASIL_EXTRACT\*" -Destination . -Recurse -Force
git add .
git commit -m "upload website PWA siap deploy"
git push origin main
```

## Aktifkan GitHub Pages

GitHub repo → Settings → Pages → Branch: `main` → `/root` → Save.

Link biasanya:
https://dika-arch.github.io/tespenjualan/

## Agar URL hilang di HP

Buka link di Chrome HP → menu titik tiga → Add to Home Screen / Tambahkan ke layar utama → buka dari icon yang muncul di layar utama.

Catatan: URL tidak bisa disembunyikan jika dibuka langsung di Chrome biasa. URL hilang hanya saat dibuka sebagai PWA dari Home Screen.
