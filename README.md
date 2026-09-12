# Akun YouTube Vault (PWA)

Duplikat dari Akun TikTok Vault, di-reskin warna merah/hitam/putih khas YouTube. Fungsinya sama persis: simpan data akun (foto, username, email/nomor, password, deskripsi, kategori custom, backup JSON/PDF, dll) — cuma ganti kulit dan judul.

## Deploy ke Vercel lewat GitHub

Sama persis kayak project TikTok Vault sebelumnya:
1. Push semua file ini ke repo GitHub **baru** (jangan ditumpuk ke repo TikTok Vault, biar gak ketuker)
2. Import ke Vercel → Framework Preset: Vite → Build Command: `npm run build` → Output Directory: `dist`
3. Deploy

## Yang beda dari versi TikTok

- Judul "Akun YouTube", warna aksen merah (bukan cyan/pink)
- Ikon app: padlock putih di atas merah (bukan logo TikTok manapun — sengaja dijauhin dari bentuk logo YouTube asli biar gak masalah hak cipta, cuma pinjem warna khasnya aja)
- Key penyimpanan data (localStorage) diganti prefix `youtube-vault-*`, jadi data project ini **gak akan campur** sama punya TikTok Vault meskipun di-deploy di HP yang sama

## Catatan

Data disimpan di `localStorage` HP/device tempat app ini diakses — permanen selama gak di-uninstall/clear data, tapi khusus per-device. Pakai fitur Backup Data (JSON) di dalam app buat mindahin manual ke device lain.
